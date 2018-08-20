FROM adoptopenjdk/openjdk10-openj9:nightly AS build

COPY . .

RUN ./mvnw clean package

RUN ls target

FROM adoptopenjdk/openjdk10-openj9:nightly AS runtime

RUN mkdir /opt/app

COPY --from=build target/demo-0.0.1-SNAPSHOT.jar /opt/app/app.jar

CMD ["java", "-jar", "/opt/app/app.jar"]

EXPOSE 8080
