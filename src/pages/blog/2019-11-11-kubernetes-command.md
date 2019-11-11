---
templateKey: blog-post
title: Kubernetes command
date: '2019-11-11 17:43'
featuredpost: true
featuredimage: /img/products-grid2.jpg
tags:
  - kubernetes
---
## Nodes
- Get all nodes of the cluster
```
kubectl get nodes
```

***

## Pods
- List all the pods in all namespaces.
```
kubectl get pods --all-namespaces
```

- list the pods in the default namespace
```
kubectl get pods
```

***

## Deployments
- get all deployments
```
kubectl get deployments
```
