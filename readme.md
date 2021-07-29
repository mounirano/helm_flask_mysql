# A Simple Project I did to try out Helm3 
## Prerequisite
- Python
- Docker
- K8s
- Helm


## Get it Running
1- Build the backend docker image:
```
cd app/backend/
chmod 700 dockerize.sh
./dockerize.sh
```

2- Deploy the app using Helm:
```
cd chart/
helm install dev hello_world
```

3- Access the backend service:
```
minikube service dev-backend
```

4- Access the database:
```
kubectl run -it --rm --image=mysql --restart=Never mysql-client -- mysql --host mysql --password=password
```