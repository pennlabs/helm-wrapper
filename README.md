# Wrapper Helm Chart

[![CircleCI](https://circleci.com/gh/pennlabs/helm-wrapper.svg?style=shield)](https://circleci.com/gh/pennlabs/helm-wrapper)

This helm chart applies whatever is provided within a `values.yaml` file. It is essentially just a wrapper to deploy K8s manifests through helm.

We currently use this helm chart to deploy Custom Resources using terraform through the helm provider. We do this because currently, the terraform kubernetes provider has no support for Custom Resources. [Here's an open issue on the topic](https://github.com/terraform-providers/terraform-provider-kubernetes/issues/215).
