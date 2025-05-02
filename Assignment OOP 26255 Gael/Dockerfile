# Use a lightweight Java runtime
FROM eclipse-temurin:17-jdk-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy your Java source files into the container
COPY src ./src

# Compile Java files into the correct directory
RUN mkdir -p out && find src -name "*.java" | xargs javac -d out

# Set the entrypoint to run your main class
CMD ["java", "-cp", "out", "Assignment.Qn1.MissionManagementMain"]