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

