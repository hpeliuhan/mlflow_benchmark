## Server setup:

Run:
`kubectl apply -f kuberentes/mlflow.yaml`
To start mlflow server

## Client setup:

Each client will run as standby pods. Customized simulation can be executed in the pods via kubernetes API.
To start pods:
`kubectl apply -f kubernetes/client.yaml`
