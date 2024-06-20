# DevOps

## Exam

- Console URL: https://console-openshift-console.apps.vuacloud.vua.cloud 
- API URL:  https://api.vuacloud.vua.cloud:6443 
- Review instructions: https://github.com/jstanesic/intro_to_devops_exam
- Cluster is accessible only from your VM in vcsa7.vua.cloud environment
- EF41F24F19

## Usefull links

- Red Hat: https://rha.ole.redhat.com/rha/app/summary
- https://k8s-docs.netlify.app/en/docs/reference/kubectl/cheatsheet/
- https://github.com/cherkavi/cheat-sheet/blob/master/kubernetes-cheat-sheet.md
- https://github.com/cherkavi/cheat-sheet/blob/master/openshift.md

## Red Hat OpenShift Key Concepts

- Pods: The smallest unit of a Kubernetes-managed containerized application. A pod consists of one or more containers.
- Deployments: The operational unit that provides granular management of a running application.
- Projects: A Kubernetes namespace with additional annotations that provide multitenancy scoping for applications.
- Routes: Networking configuration to expose your applications and services to resources outside the cluster.
- Operators: Packaged Kubernetes applications that extend cluster functions.

## RedHat - OpenShift Overview

- A container is an encapsulated process that includes the required runtime dependencies for an application to run.
- Containerization addresses the application development challenges around code portability, to aid in consistently running an application from diverse environments.
- Containerization also aims to modularize applications to improve development and maintenance on the various components of the application.
- When running containers at scale, it becomes challenging to configure and deliver high availability applications and to set up networking without a container platform, such as Kubernetes.
- Pods are the smallest organizational unit for a containerized application in a Kubernetes cluster.
- Red Hat OpenShift Container Platform (RHOCP) adds enterprise-class functions to the Kubernetes container platform to deliver the wider business needs.
- Most administrative tasks that cluster administrators and developers perform are available through the RHOCP web console.
Logs, metrics, alerts, terminal connections to the nodes and pods in the cluster, and many other features are available through the RHOCP web console.
