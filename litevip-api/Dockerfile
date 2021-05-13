FROM openjdk:8u292-jdk

ADD ./litevip-api-0.0.1-SNAPSHOT.jar litevip-api-0.0.1-SNAPSHOT.jar

ENV CLASSPATH=.:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar

EXPOSE 8858

ENTRYPOINT [ "java", "-jar", "-Dspring.profiles.active=dev", "/litevip-api-0.0.1-SNAPSHOT.jar" ]