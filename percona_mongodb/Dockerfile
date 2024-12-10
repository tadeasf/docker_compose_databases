ARG MONGODB_VERSION
ARG MONGODB_IMAGE
FROM ${MONGODB_IMAGE}:${MONGODB_VERSION}
USER root
COPY keyFile /opt/keyFile
RUN chown mongodb /opt/keyFile && chmod 400 /opt/keyFile && mkdir -p /home/mongodb/ && chown mongodb /home/mongodb
USER mongodb
