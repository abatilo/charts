# K8s debugging interview

In this gist, you'll find a kubeconfig for a cluster that's been provisioned
for you. In the cluster, there's a `default` namespace with some preconfigured
resources, but they don't seem to be working!

## The challenge

Your cluster will have a `kind: Service` defined in the `default` namespace for
an nginx container. You must fix everything that you find such that you can do
a `kubectl port-forward svc/$SERVICE_NAME 8080:80`, and then `curl
http://localhost:8080`.

## Advanced

If the `curl` works, let's take any remaining time to talk about what you'd
like to do to make the existing deployment "production ready".
