# Use JDK 21 runtime
FROM eclipse-temurin:21-jdk

# Set working directory inside container
WORKDIR /app

# Copy built JAR into container
COPY target/hobbie-0.0.1-SNAPSHOT.jar app.jar

# Expose Spring Boot default port
EXPOSE 8080

# Run Spring Boot app with limited memory (for Render free tier)
ENTRYPOINT ["java", "-Xmx256m", "-jar", "app.jar"]
