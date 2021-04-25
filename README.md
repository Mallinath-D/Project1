# A Helm Chart for microservice deployments

## Introduction

This helm chart deploys a deployement with services and ingresses for a given container, hosting a web service with the following properties:

- Configuration from environment variables
- exposes a number of ports, dependent on the container

The chart exposes port 8000 over http by default, with a load balancing service, but the ports and services are configured from a list of arbitrary length in the values file.




### Configure the chart

The following items can be set via `--set` flag during installation or configured by editing the `values.yaml` directly (need to download the chart first).


For other configurations, please see the [values.yaml](values.yaml) file. This file lists the configurable parameters of the microservice chart and the default values.

### Install the chart

Install the microservice helm chart with a release name `my-release`:

```bash
helm install my-release . 
```
