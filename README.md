# Prometheus Monitoring and Alerting Lab

This lab contains example scrape configuration and an alert rule. The Node Exporter target is illustrative and must be replaced with an authorized, reachable exporter endpoint.

## Validate configuration

With Prometheus installed:

```bash
promtool check config prometheus.yml
promtool check rules alerts.yml
```

Run Prometheus with this configuration according to your local installation method, then inspect **Status → Targets** and query `up` in the expression browser.

## Alert investigation

1. Confirm the target address and network reachability.
2. Check exporter service status and logs.
3. Review Prometheus target health and scrape errors.
4. Resolve the underlying issue, then confirm the alert clears.

This is a configuration example; no live Prometheus server or alert delivery has been configured by this repository commit.
