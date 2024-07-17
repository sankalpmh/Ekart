# Use a more recent version of Alpine Linux with OpenJDK 8
FROM openjdk:8-jdk-alpine

# Expose the port your application runs on
EXPOSE 8070

# Set environment variable for the application home directory
ENV APP_HOME /usr/src/app

# Copy your application's jar file into the container
COPY target/shopping-cart-0.0.1-SNAPSHOT.jar $APP_HOME/app.jar

# Set the working directory
WORKDIR $APP_HOME

# Specify the command to run your application
CMD ["java", "-jar", "app.jar"]
