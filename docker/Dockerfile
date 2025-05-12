FROM openjdk:21-jdk-slim

ARG IMAGE
ARG IMAGE_TAG

WORKDIR /home/wso2


COPY ./source/${IMAGE}-${IMAGE_TAG} ./temp


ENV WSO2_HOME=/home/wso2/temp


EXPOSE 9443 8243


CMD ["sh", "/home/wso2/temp/bin/api-manager.sh"]