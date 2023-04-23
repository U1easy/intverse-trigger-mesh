## Login to GKE Cluster 


        gcloud auth login

        gcloud container clusters get-credentials intverse-gke --zone us-central1 --project intverse

        https://cloud.google.com/blog/products/containers-kubernetes/kubectl-auth-changes-in-gke


## Cert Manager

        https://artifacthub.io/packages/helm/cert-manager/cert-manager

        $ kubectl apply -f https://github.com/cert-manager/cert-manager/releases/download/v1.11.1/cert-manager.crds.yaml

To install the chart with the release name my-release:

## Add the Jetstack Helm repository

    $ helm repo add jetstack https://charts.jetstack.io

    ## Install the cert-manager helm chart
    $ helm install my-release --namespace cert-manager --version v1.11.1 jetstack/cert-manager

## ArgoCD Deployment

     kubectl apply -f Install.yaml

## To Get the ArGOCD Password

    kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d

# Argocd Login CLI 


         $ argocd login argocd.gcp.intverse.io:443
