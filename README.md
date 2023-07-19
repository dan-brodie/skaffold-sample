# atd_skaffold_sample

## Getting Started

Skaffold relies on a number of tools to work.

- [skaffold](https://skaffold.dev/)
- [minikube](https://minikube.sigs.k8s.io/docs/)
- [gcloud](https://cloud.google.com/sdk/docs/install)
- [docker](https://docs.docker.com/get-docker/)

You can use a devcontainer or you can open this codebase directly in Google Cloud Shell and get to work right away.

[![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://shell.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/dan-brodie/skaffold-sample.git)

To run locally:

```
minikube start
skaffold dev
```

To run in dev:

```
gcloud container clusters get-credentials atd_skaffold_sample --region europe-west1 --project atd_skaffold_sample
skaffold dev -p dev --default-repo=gcr.io/atd_skaffold_sample
```