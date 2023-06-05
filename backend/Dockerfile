ARG BASE_IMAGE
FROM ${BASE_IMAGE}


ENV APP_NAME vote-backend-service

COPY ./target/${APP_NAME}*.jar /app/${APP_NAME}.jar
COPY ./docker-entrypoint.sh /app/docker-entrypoint.sh

WORKDIR /app

VOLUME /app/config

EXPOSE 8081

ENTRYPOINT [ "./docker-entrypoint.sh" ]
