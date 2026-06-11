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
```

## Restore dashboards
```bash
oc apply -f grafana/dashboards/wetlab-gpu-dashboard.yaml
oc apply -f grafana/dashboards/wet-lab-system-health-dashboard.yaml
```

## Raspberry Pi

Copy:

raspberry-pi/grafana-kiosk.service

Restart:
```bash
sudo systemctl daemon-reload
sudo systemctl restart grafana-kiosk.service
```
