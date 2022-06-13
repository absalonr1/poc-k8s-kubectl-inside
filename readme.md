From: https://trstringer.com/kubectl-from-within-pod/

## Create image
```
docker build -t kubectl-inside .
docker tag kubectl-inside absalon1000rr/kubectl-inside
docker push absalon1000rr/kubectl-inside

```
## Deploy an check
```
kubectl apply -f pod.yaml -n kube-system
kubectl logs internal-kubectl -n kube-system
```
## Agendamiento
prendido: 7:30am
apagado: 8pm

'15 8 * * *' : 8:15 am
'45 19 * * *': 19:45 pm

## Imagen publica en ECR (PROD account en AWS)


public.ecr.aws/u2u9u9e8/bx-kubectl-1.23.6-debian:v1
