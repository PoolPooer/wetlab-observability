# Wetlab Observability

Infrastructure as Code for the Wetlab monitoring stack.

## Components

- Grafana Dashboards
- Grafana Datasources
- Prometheus integrations
- Raspberry Pi kiosk dashboards
- GPU telemetry
- System health dashboards

## Deployment

```bash
oc project wetlab-monitoring
oc apply -f grafana/dashboards/
