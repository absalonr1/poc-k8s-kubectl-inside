From: https://trstringer.com/kubectl-from-within-pod/

## Create image
```
aws ecr-public get-login-password --region us-east-1 | docker login --username AWS --password-stdin public.ecr.aws/u2u9u9e8
docker build -t bx-kubectl-1.23.6-debian .
docker tag bx-kubectl-1.23.6-debian:latest public.ecr.aws/u2u9u9e8/bx-kubectl-1.23.6-debian:v1
docker push public.ecr.aws/u2u9u9e8/bx-kubectl-1.23.6-debian:v1

```

## Agendamiento

~~~~
  prendido: 7:30am
  apagado: 8pm
~~~~
~~~~
  '15 8 * * *' : 8:15 am
  '45 19 * * *': 19:45 pm
~~~~
## Imagen publica en ECR (PROD account en AWS)


public.ecr.aws/u2u9u9e8/bx-kubectl-1.23.6-debian:v1
