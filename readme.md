From: https://trstringer.com/kubectl-from-within-pod/

```
docker build -t kubectl-inside .
docker tag kubectl-inside absalon1000rr/kubectl-inside
docker push absalon1000rr/kubectl-inside

```

```
kubectl apply -f pod.yaml -n kube-system
kubectl logs internal-kubectl -n kube-system
```
prendido: 7:30am
apagado: 8pm

'15 8 * * *' : 8:15 am
'45 19 * * *': 19:45 pm
