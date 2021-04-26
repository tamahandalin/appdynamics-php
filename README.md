#oc new-build openjdk:8-jdk-alpine --name=appdynamics-phpagent --binary

#vi Dockerfile
FROM openjdk:8-jdk-alpine

RUN mkdir /opt/appdynamics-phpagent
ADD . /opt/appdynamics-phpagent

#oc start-build appdynamics-phpagent --from-dir . --follow

#oc new-app appdynamics-phpagent
