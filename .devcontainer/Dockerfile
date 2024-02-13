FROM mcr.microsoft.com/devcontainers/typescript-node
RUN echo "deb [trusted=yes] https://packages.twingate.com/apt/ /" | tee /etc/apt/sources.list.d/twingate.list
RUN apt-get update -yq && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install git curl
RUN curl -s https://binaries.twingate.com/client/linux/install.sh | sudo bash