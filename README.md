# lab-may-2022


This is an overview of some of my learnings from hands on exercises with CI/CD with the Harness platform and K8 with GKE.

## Overview
- [ ] Set up K8 on GKE.
- [ ] Install Harness delegate.
- [ ] Setup Harness CI.
- [ ] Setup Harness CD.

## Setting up K8 on GKE
1. Follow [GKE quickstart](https://cloud.google.com/kubernetes-engine/docs/deploy-app-cluster#standard).
2. Reuse hello-cluster created above. 
3. Run these commands to enable autoscaling on the cluster created:
```
gcloud container clusters update hello-cluster --enable-autoprovisioning --min-cpu 8 --min-memory 8 --max-cpu 12 --max-memory 24 --autoprovisioning-scopes=https://www.googleapis.com/auth/logging.write,https://www.googleapis.com/auth/monitoring,https://www.googleapis.com/auth/devstorage.read_only --zone us-west1-a
gcloud container node-pools update default-pool --enable-autoprovisioning --zone us-west1-a
```

## Install Harness delegate in GKE


## Follow Harness CI quickstart

## Follow Harness CD quickstart

## Notes
## Links
- Repository: https://github.com/parsontodd/lab-may-2022
- References:



