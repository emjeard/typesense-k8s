# typesense-kubernetes


This repo hosts kustomize files for deploying typesense in a kubernetes cluster.

> ⚠️ This approach is not reliable with more than 1 replica: https://github.com/typesense/typesense/issues/465


## Quickstart

> kubectl apply -f https://raw.githubusercontent.com/typesense/typesense-kubernetes/master/base/install.yaml
## Detailed setup:

1. Clone the repo

> git clone https://github.com/typesense/typesense-kubernetes


2. modify the overlays/dev/kustomization.yaml file according to your needs



Run below command:

To install

> kustomize build overlays/dev | kubectl apply -f - 

Clean up

> kustomize build overlays/dev | kubectl delete -f - 





