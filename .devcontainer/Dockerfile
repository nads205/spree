FROM mcr.microsoft.com/devcontainers/ruby:3.3

# Install system dependencies
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
    libpq-dev \
    postgresql-client \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/*

# [Optional] Install additional OS packages
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
    git \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/* 