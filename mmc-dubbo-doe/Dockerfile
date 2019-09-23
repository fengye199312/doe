FROM fengye199312/mvn-base:1.0
ADD target/dubbo-doe.jar /app.jar
EXPOSE 3000
RUN mkdir -p /app/doe/lib
ADD target/classes/pom.xml /app/doe
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]


