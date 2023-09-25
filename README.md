<table align="center"><tr><td align="center" width="9999">
<img src="icons/prometheus_grafana_logo.png" align="center" width="150" alt="Docker icon">

# prometheus-grafana-alertmanager

</td></tr></table>

Simple project with a single docker-compose.yml file for deploying Prometheus, Grafana, Alertmanager monitoring stack
behind Traefik reverse proxy in Docker SWarm environment.

# Deploy stack

```sh
docker stack deploy -c ./docker-compose.yml prometheus-grafana-alertmanager
```

# Exposed user interfaces

Based on Traefik routers and middlewares configuration, the exposed UIs of deployed services:
- `Traefik`: https\://host/dashboard/#/
- `Prometheus`: https\://host/prometheus
- `Grafana`: https\://host/grafana
- `Alertmanager`: https\://host/alertmanager

