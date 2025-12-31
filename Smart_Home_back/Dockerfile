# ==============================
# Stage 1: Build with Maven
# ==============================
FROM maven:3.8.4-eclipse-temurin-17 AS builder
WORKDIR /app

COPY pom.xml .
COPY src ./src

RUN mvn clean package -DskipTests

# ==============================
# Stage 2: Runtime image
# ==============================
FROM eclipse-temurin:17-jdk-alpine
VOLUME /tmp

WORKDIR /app
COPY --from=builder /app/target/*.jar app.jar

ENTRYPOINT ["java","-jar","app.jar"]