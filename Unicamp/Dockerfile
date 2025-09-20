FROM openjdk:11-jdk-slim

WORKDIR /app

# copie os fontes (caminhos RELATIVOS à pasta Unicamp/, que é o contexto)
COPY src/main/java ./src/main/java

# compile tudo para /app/out (inclui Main.java e OlaUnicamp.java)
RUN mkdir -p out \
 && javac -encoding UTF-8 -d out $(find src/main/java -name "*.java")

# execute a classe pelo nome totalmente qualificado
CMD ["java", "-cp", "out", "org.example.OlaUnicamp"]
