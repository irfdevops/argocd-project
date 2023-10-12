# Use a minimal base image with Java
FROM adoptopenjdk/openjdk11:alpine-jre

# Set the working directory in the container
WORKDIR /app

# Copy the JAR file from the project's target directory to the container
COPY target/spring-boot-web.jar app.jar

# Define the command to run your Java application
ENTRYPOINT ["sh", "-c", "java ${JAVA_OPTS} -jar app.jar"]
