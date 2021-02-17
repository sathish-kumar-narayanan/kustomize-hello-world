# kustomize-hello-world

A simple hello world kustomize deployments

## Steps to build

- ` kustomize build base `
- ` kustomize build overlays/staging `
- ` kustomize build overlays/production `

## steps to deploy

- ` kubectl create namespace <your-name> `
- ` kustomize build overlays/staging | kubectl apply -f - -n <your_name> `

# Reference
- source: https://github.com/kubernetes-sigs/kustomize/tree/master/examples/helloWorld
- container source: https://github.com/monopole/hello
