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
helm install release_name hello_world
```