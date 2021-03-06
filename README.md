# Fluentd Monitoring Mixin for OpenShift Aggregated Logging

> NOTE: This project is *alpha* stage. Flags, configuration, behaviour and design may change significantly in following releases.

A set of Grafana dashboard and Prometheus alerts for Fluentd deployed as part of [Origin-Aggregated-Logging](https://github.com/openshift/origin-aggregated-logging/).

## How to use

This repository has been heavily inspired by <https://github.com/kubernetes-monitoring/kubernetes-mixin>.
Follow that repository for further information about deployment.

### Quick and dirty hint

```
$ make clean && make

# Prometheus rules and alerts are generated here:
$ file ./prometheus_rules.yaml ./prometheus_alerts.yaml 
./prometheus_rules.yaml:  ASCII text
./prometheus_alerts.yaml: ASCII text

# dashboard json is generated here:
$ file dashboards_out/fluentd.json 
dashboards_out/flunetd.json: ASCII text 
```