FROM openjdk:8u292-jdk

ENV CLASSPATH=.:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar
VOLUME /tmp
ADD rocketmq-console-ng-*.jar rocketmq-console-ng.jar
RUN sh -c 'touch /rocketmq-console-ng.jar'
ENV JAVA_OPTS=""
EXPOSE  8070
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -jar /rocketmq-console-ng.jar" ]