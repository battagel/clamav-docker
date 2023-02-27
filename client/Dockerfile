FROM debian:latest

# Update package list and install basic packages
RUN apt-get update && \
    apt-get install -y \
    curl \
    wget \
    vim \
    nano \
    net-tools \
    iputils-ping \
    sudo \
    clamav-daemon


# Clean up package cache
RUN apt-get clean && \
    rm -rf /var/lib/apt/lists/*

COPY clamd.conf /etc/clamav/clamd.conf
