FROM openjdk:21-slim
RUN apt-get update && \
    apt-get install -y curl wget vim git jq bash bash-completion tcpdump && \
    apt-get autoclean && \
    apt-get autoremove && \
    mkdir -p /opt/app && \
    useradd -ms /bin/bash usrapp && \
    chown -R usrapp /opt/
WORKDIR /opt/app
EXPOSE 8080
USER usrapp
