faced issue while frontend accessing the API from my browser (which is in diffrenet network)

resolved it my exposing the api deployment and used the exposed port 

Kubernetes-Manifests-file/Frontend/deployment.yaml

(http://<NODE_IP>:PORT/api/tasks)

utill now used the hard coded ip value in as (env) in frontend/deployment.yaml
when the deploying hardware ip changes then i have to rebuild the image to access the backend through browser due to the ENV is directly adding while build process

now adding the ingress controller to cluster and using the routing paths to access

adding the domain to /etc/hosts for testing purpose

"http://api:3500/api/tasks" -- refer -- three-tier-ingress.yaml
