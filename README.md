# Kubernetes Example Cluster

This is the repository for the main example cluster described in the book, "Cloud Native Applications with Docker and Kubernetes" by Jonathan Bartlett.

To run this cluster

* Create a Kubernetes cluster (on Linode.com, for instance)
* export the environment variable `KUBECONFIG` to point to the kubeconfig file for the cluster.
* Install the main application: `kubectl apply -f .`
* Install the environment-specific configurations: `kubectl apply -f environments/production`
* Install the secrets: `kubectl apply -f secrets`
* Install the nginx Ingress: `kubectl apply -f https://bit.ly/ingress_nginx_1_2_0`

# Other Branches

Other branches have other versions of the cluster:

* The `simple-cluster` branch has the code from Chapter 9, "Basic Kubernetes Management."
