# grafana-agent-rock

[![Open a PR to OCI Factory](https://github.com/canonical/grafana-agent-rock/actions/workflows/rock-release-oci-factory.yaml/badge.svg)](https://github.com/canonical/grafana-agent-rock/actions/workflows/rock-release-oci-factory.yaml)
[![Publish to GHCR:dev](https://github.com/canonical/grafana-agent-rock/actions/workflows/rock-release-dev.yaml/badge.svg)](https://github.com/canonical/grafana-agent-rock/actions/workflows/rock-release-dev.yaml)
[![Update rock](https://github.com/canonical/grafana-agent-rock/actions/workflows/rock-update.yaml/badge.svg)](https://github.com/canonical/grafana-agent-rock/actions/workflows/rock-update.yaml)

[Rocks](https://canonical-rockcraft.readthedocs-hosted.com/en/latest/) for [Grafana Agent](https://grafana.com/oss/agent/).  
This repository holds all the necessary files to build rocks for the upstream versions we support. The Grafana Agent rock is used by the [grafana-agent-k8s-operator](https://github.com/canonical/grafana-agent-k8s-operator) charm.

The rocks on this repository are built with [OCI Factory](https://github.com/canonical/oci-factory/), which also takes care of periodically rebuilding the images.

Automation takes care of:

* validating PRs, by simply trying to build the rock;
* pulling upstream releases, creating a PR with the necessary files to be manually reviewed;
* releasing to GHCR at [ghcr.io/canonical/grafana-agent:dev](https://ghcr.io/canonical/grafana-agent:dev), when merging to main, for development purposes.

