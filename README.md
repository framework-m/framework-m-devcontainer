# Framework M Devcontainer

## Introduction

Welcome to the **Framework M** developer container! This repository is designed to be a zero-config, "one-click" environment for building modular business applications.

## Getting Started (Daytona / Gitpod / Codespaces)

1.  **Open in Cloud IDE**: Just click the "Open" button in your favorite provider.
2.  **Wait for Setup**: The devcontainer will automatically sync dependencies and link the `m` CLI.
3.  **Create Your First App**:
    ```bash
    uv run m new app my-cool-app --with-frontend
    ```
4.  **Run prerequisite commands**:
    ```bash
    cd my_cool_app
    uv add psycopg2-binary
    uv run m migrate init
    uv run m migrate all
    ```
5.  **Start Developing**:
    ```bash
    uv run m dev --studio
    ```

## Features

- **Metadata-Driven**: Define your data models (DocTypes) in Python, and the framework handles the rest.
- **Unified Frontend**: Instant React/Vite frontends with built-in desk UI.
- **Enterprise-Ready Infrastructure**:
  - **PostgreSQL 16**: High-performance analytical and transactional storage.
  - **Redis 7**: Fast caching and built-in pub/sub.
  - **NATS 2**: Modern enterprise-grade event bus.
- **Built-in Studio**: A developer portal available on port `9999`.

## Architecture Modes

- **Indie Mode**: Default with SQLite (internal) or local files.
- **Enterprise Mode**: Enabled by default in this devcontainer, utilizing Postgres, Redis, and NATS for scale.

Enjoy the frictionless developer experience!
