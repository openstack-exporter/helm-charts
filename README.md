# Helm Chart for OpenStack Exporter

## Description

This is the official Helm Chart for [OpenStack Exporter](https://github.com/openstack-exporter/openstack-exporter), a tool to export Prometheus metrics from a running OpenStack Cloud.

## Configuration

The chart configuration is done in the `values.yaml` file.

## Usage

```bash
# Get a local copy
git clone https://github.com/openstack-exporter/helm-charts.git

# Package the chart
cd helm-charts/charts/prometheus-openstack-exporter/
helm package . 

# Get chart version & install
version="$(awk '/^version:/{ print $NF }' Chart.yaml)"
helm install prometheus-openstack-exporter prometheus-openstack-exporter-${version}.tgz
```

## Contributing

Please fill pull requests or issues under Github.
