# Gaetan UBIQuitous Homelab

Welcome to my **GUBIQH** configuration repository! This repo contains all the configuration files, deployment scripts, and documentation for managing my home server infrastructure. The setup is orchestrated using [Docker Compose](https://docs.docker.com/compose/) and includes several containerized services.

---

## 📚 Table of Contents

- [Architecture Overview](#architecture-overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Configuration](#configuration)
- [Services](#services)
- [Backups & Maintenance](#backups--maintenance)
- [Roadmap / TODO](#roadmap--todo)

---

## 🏗️ Architecture Overview

**TODO**
Below is an overview of my homelab architecture.  
![Homelab Architecture](./assets/architecture.png)
<!-- Replace with the actual path to your image -->

---

## 🚀 Getting Started

### Prerequisites

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

### Clone the Repository

```bash
git clone https://github.com/gdufay/homelab.git
cd homelab
```

### Start the Stack

```bash
docker compose up -d
```

---

## ⚙️ Configuration

- All configuration files (e.g., `.env`, `compose.yml`, custom Dockerfile) are located in this repository.
- Review and edit `.env.example` to set up environment-specific variables.
- Sensitive information should be stored in a separate `.env` file, which is **not** committed to version control.

---

## 🧩 Services

Includes the following containers:

| Service Name                                                             | Description                            | Domain      |
|--------------                                                            |---------------------------------       |---------    |
| [caddy-docker-proxy](https://github.com/lucaslorentz/caddy-docker-proxy) | Reverse Proxy & SSL with docker labels |             |
| [homepage](https://gethomepage.dev)                                      | Dashboard                              |             |
| [actual-budget](https://actualbudget.org)                                | Finance management                     | budget      |
| [pocket-id](https://pocket-id.org)                                       | OIDC provider                          | pocket-id   |
| [immich](https://docs.immich.app)                                        | Photo and video management             | immich      |
| [spoolman](https://github.com/Donkie/Spoolman)                           | 3D-printer filament spools tracker     | spoolman    |
| [vaultwarden](https://github.com/dani-garcia/vaultwarden)                | Secure vault                           | vaultwarden |
| [grafana](https://grafana.com/docs)                                      | Monitoring and visualisation           | grafana     |
| [prometheus](https://prometheus.io)                                      | Metrics and monitoring                 | prometheus  |
| [freshRSS](https://freshrss.org)                                         | RSS aggregator                         | rss         |

---

## 🔄 Backups & Maintenance

**TODO**

- Define backup strategy for persistent volumes and configuration files.
- Document backup scripts and procedures.

---

## 🗺️ Roadmap / TODO

- [ ] Document and automate backup & restore procedures
- [ ] Improve monitoring & alerting stack (e.g., Prometheus, Grafana)
- [ ] Improve security
- [ ] Add more services as needed (update services section)
- [ ] Implement CI/CD for config changes
- [ ] Open to the world
