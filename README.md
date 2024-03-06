# ArgoCD + K8s + Bookinfo

See: [deploying-microservice-application-argocd-kubernetes](https://tech-skill-forge.vercel.app/challenges/deploying-microservice-application-argocd-kubernetes)

## Problem

Modern software development requires robust deployment strategies that can handle the dynamic nature of containerized applications. Kubernetes offers a scalable platform for managing containerized applications, but managing deployments can become complex. ArgoCD, a declarative GitOps continuous delivery tool for Kubernetes, simplifies this process enabling developers to automate and manage deployments using Git as the source of truth.

## Starting Point

The Bookinfo application is broken into four separate microservices:

![bookinfo-architecture](https://istio.io/latest/docs/examples/bookinfo/noistio.svg)

- `productpage`. The `productpage` microservice calls the `details` and `reviews` microservices to populate the page.
- `details`. The `details` microservice contains book information.
- `reviews`. The `reviews` microservice contains book reviews. It also calls the `ratings` microservice.
- `ratings`. The `ratings` microservice contains book ranking information that accompanies a book review.

This repository contains the K8s manifests for deploying the Bookinfo application to a Kubernetes cluster. The manifests are organized into separate directories within [bookinfo/](./bookinfo/) for each microservice.





