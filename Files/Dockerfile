#java runtime environment for our project
FROM openjdk:8-jre-alpine

#creating non-root user
RUN adduser --disabled-password --gecos "" petclinic
USER petclinic
WORKDIR /home/petclinic

#copying file from host to image
COPY petclinic.jar .

#the command to be run when container starts
CMD java -jar petclinic.jar

#exposing port
EXPOSE 8080
