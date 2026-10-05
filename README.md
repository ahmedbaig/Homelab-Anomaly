# homelab-anomaly

Anomaly detection for my home lab: logs first, then network and metrics, with retraining and alerting.

Builds on [proxmox](https://github.com/ahmedbaig/proxmox), which already describes the infrastructure, and on the Loki logs and Prometheus metrics the lab already collects.

## Phases

1. **Log anomaly detector:** a small language model over the home lab logs.
2. **Network and metrics:** add DNS flow, network and Prometheus signals.
3. **Operate:** scheduled retraining and alerts through the existing Alertmanager.
