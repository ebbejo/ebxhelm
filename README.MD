# oc - simple Docker container with Helm

1. Build

```
    docker build -t quay.io/ebbe_jonsson/ebxhelm .
```

2. Set up alias:

```
alias helm='docker run --rm -ti -v /etc/hosts:/etc/hosts:ro -v $(pwd):/files -v $(pwd)/.kube:/root/.kube quay.io/ebbe_jonsson/ebxhelm'
```
