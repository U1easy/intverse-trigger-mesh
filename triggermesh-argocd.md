### Trigger Mesh Installation Via ArgoCD

1. Knative Operator

        https://34.134.84.58/applications/argocd/knative-operator?view=tree&resource=
 
        kubectl apply -f https://github.com/IntVerse/intverse-trigger-mesh/blob/main/argocd/applications/triggermesh-stack/knative-operator.yaml

 2. Knative Serving 

        https://34.134.84.58/applications/argocd/knative-serving?view=tree&resource=

        kubectl apply -f  https://github.com/IntVerse/intverse-trigger-mesh/blob/main/argocd/applications/triggermesh-stack/knative-serving.yaml

3. TriggerMesh CRDs & TriggerMesh controllers

        https://34.134.84.58/applications/argocd/trigger-mesh?view=tree&resource=
      
        kubectl apply -f https://github.com/IntVerse/intverse-trigger-mesh/blob/main/argocd/applications/triggermesh-stack/triggermesh.yaml

4. TriggerMesh Telemetry Components

    Logging:- 

        https://34.134.84.58/applications/argocd/triggermesh-logging?view=tree&resource=

        kubectl apply -f https://github.com/IntVerse/intverse-trigger-mesh/blob/main/argocd/applications/triggermesh-telemetery/triggermesh-logging.yaml
  
    
    Metrics :- 

        https://34.134.84.58/applications/argocd/triggermesh-metrics?view=tree&resource=

        kubectl apply -f https://github.com/IntVerse/intverse-trigger-mesh/blob/main/argocd/applications/triggermesh-telemetery/triggermesh-metrics.yaml