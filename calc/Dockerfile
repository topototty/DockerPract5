FROM ubuntu:latest

RUN apt-get update && apt-get install -y \
    openjdk-17-jre \
    && rm -rf /var/lib/apt/lists/*

COPY calc.jar /app/calc.jar

WORKDIR /app

ENV DISPLAY=host.docker.internal:0

CMD ["java", "-jar", "calc.jar"]
