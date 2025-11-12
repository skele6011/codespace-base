# Base image: lightweight Ubuntu with devcontainer support
FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Set noninteractive mode for apt-get (lowk dk what this does)
ENV DEBIAN_FRONTEND=noninteractive

# Install system packages
RUN apt-get update && apt-get install -y --no-install-recommends \
    git \
    curl \
    wget \
    unzip \
    build-essential \
    python3 \
    python3-pip \
    openjdk-17-jdk \
    nodejs \
    npm \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN npm install -g http-server

# Set JAVA_HOME environment variable for Java extensions in VS Code
ENV JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64
ENV PATH=$JAVA_HOME/bin:$PATH

# Set the default workspace folder
WORKDIR /workspaces

# Default command (should be allowed to be overridden by codespace)
CMD [ "bash" ]
