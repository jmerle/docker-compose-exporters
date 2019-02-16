# Docker Compose Exporters

A Docker Compose configuration to run various [Prometheus](https://prometheus.io/) exporters, to be used by a Prometheus server that is running behind a [Traefik](https://traefik.io/) reverse proxy.

## Usage

1. Clone this repository.
2. Copy `.env.example` to `.env` and modify the variables.
3. Copy `blackbox-example` to `blackbox` and adapt it's configuration to your needs.
4. Run `docker-compose up -d`.

## Exporters

The Docker Compose configuration includes the following exporters:
- [Node Exporter](https://github.com/prometheus/node_exporter) on port 9100
- [cAdvisor](https://github.com/google/cadvisor) on port 8080
- [Blackbox Exporter](https://github.com/prometheus/blackbox_exporter) on port 9115
