FROM openjdk:17-jdk-slim
RUN mkdir -p /app
COPY vizucar-api /app/vizucar-api
RUN chmod +x /app/vizucar-api/mvnw
RUN ./mvnw clean package
EXPOSE 80
CMD ["sh", "-c", "java -jar /app/vizucar-api/target/*.jar"]