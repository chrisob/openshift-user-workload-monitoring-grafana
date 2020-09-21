# Grafana example for OpenShift User Workload Monitoring

This repo contains a Kustomize base and example overlay which deploys a
proof-of-concept Grafana instance which is configured to "plug-in" to OpenShift
Container Platform's [user workload monitoring stack][user-workload-monitoring].

The generated manifests have been tested against OpenShift Container Platform
v4.5.12. Breaking changes in higher versions may also break this Grafana
instance.

## Why?

Because the user workload monitoring stack is still an early tech-preview, there
is no support for user-provided Grafana dashboards. Even though metrics scraping
and alerting is provided out-of-the-box, most of the applications/operators I
support need a friendly dashboard to take up screen real-estate :grin:.


[user-workload-monitoring]:https://docs.openshift.com/container-platform/4.5/monitoring/monitoring-your-own-services.html
