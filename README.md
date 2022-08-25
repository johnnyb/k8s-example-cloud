# Simple Deployment

This code is just a simple example deployment.  
You can install this by simply doing: `kubectl apply -f .`

To find the IP address that this is listening on, do: `kubectl get services`

Note that the Pod defined in `simple-pod.yaml` will be running, since there is no service connected to it the Pod is not accessible.
