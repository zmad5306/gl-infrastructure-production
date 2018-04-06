# gl-infrastructure-production
k8s manifests for production env

## Create Cluster

`gcloud config set compute/zone us-central1-f`

`gcloud container clusters create production --cluster-version=1.9.4-gke.1 --node-version=1.9.4-gke.1 --num-nodes=4`

## Create Static IP

`gcloud compute addresses create gl-production-ip --global`