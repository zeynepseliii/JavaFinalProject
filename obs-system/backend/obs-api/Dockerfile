# Temel imaj
FROM openjdk:17

# JAR dosyasını konteynıra kopyala
COPY target/*.jar /app.jar

# Portu belirt
EXPOSE 8080

# Uygulamayı çalıştır
ENTRYPOINT ["java", "-jar", "/app.jar"]