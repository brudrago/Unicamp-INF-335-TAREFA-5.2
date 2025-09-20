FROM openjdk:11-jdk-slim

WORKDIR /app/Unicamp

# copia seu fonte
COPY Unicamp/OlaUnicamp.java .

# compila
RUN javac OlaUnicamp.java

# executa
CMD ["java", "OlaUnicamp"]
