# DC Residency

OpenShift Gitops Operator was already deployed, so we are only installing an ArgoCD instance, without the operator.

``` 
helm upgrade --install argocd -f argocd-values.yaml --create-namespace   --namespace labs-ci-cd  --set operator=false redhat-cop/gitops-operator
``` 
