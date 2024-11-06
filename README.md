# Kustomize and its Uses

Kustomize is a k8s manifest system that can add, remove, or update configuration options in a DRY method. Unlike Helm, it directly modifies the YAML files to produce output that is then fed to the k8s API.

Additional information can be found [here](https://kubernetes.io/docs/tasks/manage-kubernetes-objects/kustomization/).

To get started, clone this repo, install kubectl & kustomize, and you can start playing with it in your local minikube instance (or wherever else you use kubernetes.)

To test it out, you can output a yaml file with `kustomize build overlays/dev` from within the `kustomize` directory to output an updated yaml manifest for an example development environment.

For a bit more involvement, you can use `kubectl apply -k overlays/dev` to apply the dev manifest to your cluster of choice.

Happy hacking!
