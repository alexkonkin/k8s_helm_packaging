# k8s_helm_packaging
to build package
1. check if it is valid and does not have syntax errors
  helm lint <packagename>
2. create package
  helm package <packagename>

to install the package we can use the next commands:
1.
expose our local repository (~/.helm) via http:
helm serve&
2.
install petclinic package
helm install petclinic --name=petclinic
