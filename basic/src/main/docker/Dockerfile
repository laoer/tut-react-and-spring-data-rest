FROM java:8
VOLUME /tmp
ADD react-and-spring-data-rest-basic-0.0.1-SNAPSHOT.jar app.jar
RUN bash -c 'touch /app.jar'
EXPOSE 8701

ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]

# Expose our log volumes
#VOLUME ["/data"]
#ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar","--log.path=/data"]
