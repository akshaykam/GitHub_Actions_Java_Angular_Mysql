FROM openjdk:8
WORKDIR /app
COPY ./target/springboot-backend-0.0.1-SNAPSHOT.jar /app
RUN sudo apt update
RUN sudo apt install maven -y
RUN mvn -version
CMD ["java","-jar","springboot-backend-0.0.1-SNAPSHOT.jar"]