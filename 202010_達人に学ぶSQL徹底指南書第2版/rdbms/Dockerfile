FROM postgres:latest
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && \
    apt-get install -y build-essential cmake clang libssl-dev vim openssh-server iputils-ping net-tools

RUN mkdir /src

WORKDIR /src

EXPOSE 5432