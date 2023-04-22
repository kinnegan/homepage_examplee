just for testing k8s cluster and IngressController
first of all - build new docker image and push it int to registry:
 - docker build -t <YOUR REPO HERE>/<APP NAME>:<TAG> .
 - docker push <YOUR REPO HERE>/<APP NAME>:<TAG>
Change FQDN hostname and another stuff in test-k8s-application.yaml and run it:
 - kubectl apply -f test-k8s-application.yaml
