# wa-api

A lightweight WhatsApp API service to send and receive messages via a backend API. This repository provides a Dockerized service and environment-based configuration for easy deployment.

---

## About this project ✅

This project implements a WhatsApp API backend (named `wa-api`) that exposes HTTP endpoints to interact with WhatsApp programmatically. It's designed to be simple to run locally or in a containerized environment and to be configured via environment variables.

---

## Feature ✨

- Send and receive WhatsApp messages
- Webhook / callback support for inbound messages
- Docker Compose setup for quick start
- Environment-based configuration via `.env`

---

## How to install 🔧

### Prerequisites

- Git
- Docker & Docker Compose (or Docker Desktop)

### Steps

1. Clone the repository

```bash
git clone <repo-url>
cd wa-api
```

2. Configure environment

- Generate a .env file:

```bash
docker compose run --no-deps -v "$(pwd)":/app/env waha init-waha /app/env
```

- Otherwise, create a `.env` file in the project root and set the required variables (API keys, ports, database URIs, etc.).

3. Run with Docker Compose (recommended)

```bash
docker compose up -d
```

Check logs:

```bash
docker compose logs -f
```

---

## Usage 💡

- After the service starts, use the documented HTTP endpoints to send messages or register webhooks.
- Update `.env` as needed for credentials and ports.

---

## Contributing 🤝

Contributions are welcome — please open issues or pull requests with improvements or bug fixes.

---

## License

Add a license file or statement here as appropriate.
