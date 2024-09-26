# Base image for Java
FROM adoptopenjdk/openjdk11:alpine-jre

# Set artifact path relative to the build context
ARG artifact=target/spring-boot-web.jar

# Set the working directory
WORKDIR /opt/app

# Copy the JAR file from the target directory in the build context
COPY ${artifact} app.jar

# Command to run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
