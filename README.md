## Server setup:

Run:
`kubectl apply -f kuberentes/mlflow.yaml`
To start mlflow server

## Client setup:
Build docker images:
`docker build -t mlflow-client:latest .`
`docker tag mlflow-client:latest localhost:5000/mlflow-client:latest`
`docker push localhost:5000/mlflow-client:latest`

Each client will run as standby pods. Customized simulation can be executed in the pods via kubernetes API.
To start pods:
`kubectl apply -f kubernetes/client.yaml`
