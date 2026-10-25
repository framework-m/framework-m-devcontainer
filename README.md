# Framework M Devcontainer

A zero-config devcontainer for building Framework M applications.

## What's included

- Python 3.12 + uv (with the `m` CLI linked)
- Node 24 + pnpm
- PostgreSQL 16, Redis 7, and NATS 2
- Forwarded ports: 8000 (m prod), 8888 (API), 5173 (Vite), 9999 (Studio)
- VS Code extensions for Python, Pylance, Prettier, and ESLint

## Get started

- [Framework M Getting Started](https://www.frameworkm.dev/docs/tutorials/getting-started) — create and run an app.
- [Develop in a Devcontainer](https://www.frameworkm.dev/docs/tutorials/develop-in-a-devcontainer) — open this repo with VS Code Dev Containers or Devsy.

The devcontainer runs in enterprise mode: PostgreSQL, Redis, and NATS are configured automatically.
