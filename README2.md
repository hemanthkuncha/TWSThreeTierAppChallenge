faced issue while frontend accessing the API from my browser (which is in diffrenet network)

resolved it my exposing the api deployment and used the exposed port 

Kubernetes-Manifests-file/Frontend/deployment.yaml

(http://<NODE_IP>:PORT/api/tasks)
