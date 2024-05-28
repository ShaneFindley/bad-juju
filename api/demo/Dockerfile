# Start with a base image containing Java runtime
FROM openjdk:21-ea-26-jdk-oracle

# Add Maintainer Info
LABEL maintainer="email@example.com"

# Make port 8080 available to the world outside this container
EXPOSE 8080

# The application's jar file
ARG JAR_FILE=build/libs/demo-0.0.1-SNAPSHOT.jar

# Add the application's jar to the container
ADD ${JAR_FILE} demo.jar

# Run the jar file 
ENTRYPOINT ["java","-jar","/demo.jar"]