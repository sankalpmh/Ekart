# Use a more recent version of Alpine Linux with OpenJDK 8
FROM openjdk:8-jdk-alpine

# Set environment variables
ENV APP_HOME /usr/src/app
ENV JAVA_OPTS=""

# Expose the port your application runs on
EXPOSE 8070

# Copy your application's jar file into the container
COPY target/shopping-cart-0.0.1-SNAPSHOT.jar $APP_HOME/app.jar

# Set the working directory
WORKDIR $APP_HOME

# Specify the command to run your application
CMD ["sh", "-c", "java $JAVA_OPTS -jar app.jar"]

# Use ENTRYPOINT instead of CMD if you need to pass additional arguments when starting the container
# ENTRYPOINT ["sh", "-c", "java $JAVA_OPTS -jar app.jar"]

