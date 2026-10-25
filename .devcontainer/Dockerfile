FROM mcr.microsoft.com/devcontainers/python:3.12

# Install uv for fast python package management
RUN curl -LsSf https://astral.sh/uv/install.sh | sh && \
    mv /root/.local/bin/uv /usr/local/bin/uv

# Install Node.js and pnpm for frontend development
RUN curl -fsSL https://deb.nodesource.com/setup_24.x | bash - && \
    apt-get install -y nodejs && \
    npm install -g pnpm

# Set up workdir
WORKDIR /workspace
