FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD gateway-1.0.0.jar gateway-1.0.0.jar
RUN sh -c 'touch /gateway-1.0.0.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /gateway-1.0.0.jar" ]
