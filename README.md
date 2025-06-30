# Monitoring Lab

This project provides a complete Docker Compose setup for monitoring using Loki and Promtail. Kubernetes is not required—everything runs with Docker Compose for simplicity and ease of use.

**Developed and maintained by Aqib Hafeez (DevOps Engineer).**
## Features

- **Loki**: Log aggregation system that stores and queries logs efficiently.
- **Promtail**: Agent that ships the contents of local logs to Loki.
- **Docker Compose**: Simplifies deployment and management of monitoring stack.

## Getting Started

### Prerequisites

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/)

### Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/monitoring-lab.git
    cd monitoring-lab
    ```
2. Start the monitoring stack:
    ```bash
    docker-compose up -d
    ```

### Accessing the Services

- **Loki**: [http://localhost:3100](http://localhost:3100)
- **Promtail**: Runs as a background service, no direct UI.

## Folder Structure

```
.
├── docker-compose.yml
├── loki-config.yaml
├── promtail-config.yaml
└── README.md
```

## Configuration

- **loki-config.yaml**: Loki configuration file.
- **promtail-config.yaml**: Promtail configuration file.
- **docker-compose.yml**: Service definitions.

## Stopping the Stack

To stop and remove the containers:
```bash
docker-compose down
```

## License

This project is licensed under the MIT License.