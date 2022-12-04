# See here for image contents: https://github.com/microsoft/vscode-dev-containers/blob/v0.202.3/containers/python-3/.devcontainer/base.Dockerfile
# [Choice] Python version (use -bullseye variants on local arm64/Apple Silicon): 3, 3.9, 3.8, 3.7, 3.6, 3-bullseye, 3.9-bullseye, 3.8-bullseye, 3.7-bullseye, 3.6-bullseye, 3-buster, 3.9-buster, 3.8-buster, 3.7-buster, 3.6-buster
ARG VARIANT=3-bullseye
FROM mcr.microsoft.com/devcontainers/python:0-${VARIANT}

RUN pip3 install --upgrade youtube-dl moviepy

# Install Dependancies
RUN apt-get update && apt-get install -y \
    ffmpeg \
    vim \
    curl \
    tar \
    file \
    xz-utils \
    build-essential \
    uuid-runtime \
    && rm -rf /var/lib/apt/lists/*

    # Install Dependancies
RUN apt-get update && apt-get install -y \
    imagemagick libmagickwand-dev \
    && rm -rf /var/lib/apt/lists/*

