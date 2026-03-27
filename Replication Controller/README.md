# Kubernetes Relication Controller
---
## Write rc Yaml File 
~~~sh
nano rc.yaml
~~~
~~~sh
apiVersion: v1
kind: ReplicationController
metadata:
  name: test-rc
  namespace: test
spec:
  replicas: 3
  selector:
    app: test-app
  template:
    metadata:
      labels:
        app: test-app
    spec:
      containers:
      - name: test-container
        image: nginx
        ports:
        - containerPort: 80
~~~
## Apply rc yaml file
~~~sh
kubectl apply -f rc.yaml
~~~
## Check rc
~~~sh
kubectl get rc
~~~
