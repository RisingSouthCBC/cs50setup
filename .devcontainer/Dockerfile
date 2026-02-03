FROM mcr.microsoft.com/devcontainers/python:3.11

# Avoid interactive prompts
ENV DEBIAN_FRONTEND=noninteractive

# Install system dependencies
RUN apt-get update && apt-get install -y \
    git \
    curl \
    build-essential \
    libsqlite3-dev \
    && rm -rf /var/lib/apt/lists/*

# Upgrade pip
RUN pip install --upgrade pip

# Install CS50 tools
RUN pip install \
    cs50 \
    check50 \
    submit50 \
    style50 \
    pytest
