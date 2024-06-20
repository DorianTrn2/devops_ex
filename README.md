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
- OpenShift uses Kubernetes to manage pods. Pods consist of one or more containers that share resources, such as selected namespaces and networking, and represent a single application.
- Pods are the smallest organizational unit for a containerized application in a Kubernetes cluster.
- Red Hat OpenShift Container Platform (RHOCP) adds enterprise-class functions to the Kubernetes container platform to deliver the wider business needs.
- Most administrative tasks that cluster administrators and developers perform are available through the RHOCP web console.
Logs, metrics, alerts, terminal connections to the nodes and pods in the cluster, and many other features are available through the RHOCP web console.

________________________________
### Structure Typique d'un Kubernetes Cheat Sheet

Un cheat sheet Kubernetes est généralement une référence rapide qui couvre les commandes et concepts essentiels pour travailler avec Kubernetes. Voici une structure typique que tu pourrais trouver :

1. **Introduction**
   - Bref aperçu de Kubernetes et de son utilité.

2. **Commandes de Base kubectl**
   - **Cluster Info** : `kubectl cluster-info`
   - **Get Resources** : `kubectl get [resource]`
   - **Describe Resources** : `kubectl describe [resource] [name]`
   - **Create Resources** : `kubectl create -f [file.yaml]`
   - **Delete Resources** : `kubectl delete [resource] [name]`
   - **Apply Configuration** : `kubectl apply -f [file.yaml]`

3. **Gestion des Pods**
   - **Lister les Pods** : `kubectl get pods`
   - **Décrire un Pod** : `kubectl describe pod [name]`
   - **Logs des Pods** : `kubectl logs [pod-name]`
   - **Exécuter une commande dans un Pod** : `kubectl exec -it [pod-name] -- [command]`

4. **Services et Networking**
   - **Lister les Services** : `kubectl get svc`
   - **Créer un Service** : `kubectl expose pod [pod-name] --port=[port] --target-port=[target-port]`
   - **Décrire un Service** : `kubectl describe svc [service-name]`

5. **Déploiements et Réplication**
   - **Créer un Déploiement** : `kubectl create deployment [name] --image=[image]`
   - **Mettre à jour un Déploiement** : `kubectl set image deployment/[name] [container-name]=[new-image]`
   - **Mise à l'échelle** : `kubectl scale deployment [name] --replicas=[count]`

6. **Volumes et Stockage**
   - **Lister les Volumes** : `kubectl get pv`
   - **Créer un Persistent Volume** : `kubectl create -f [pv.yaml]`
   - **Créer un Persistent Volume Claim** : `kubectl create -f [pvc.yaml]`

7. **Namespaces**
   - **Lister les Namespaces** : `kubectl get namespaces`
   - **Créer un Namespace** : `kubectl create namespace [name]`
   - **Changer de Namespace** : `kubectl config set-context --current --namespace=[name]`

8. **Configurations et Secrets**
   - **Créer une ConfigMap** : `kubectl create configmap [name] --from-literal=[key]=[value]`
   - **Créer un Secret** : `kubectl create secret generic [name] --from-literal=[key]=[value]`

9. **RBAC (Role-Based Access Control)**
   - **Lister les Roles** : `kubectl get roles`
   - **Créer un Role** : `kubectl create role [name] --verb=[verb] --resource=[resource]`

10. **Debugging et Monitoring**
    - **Trouver des erreurs** : `kubectl get events`
    - **Analyser les logs** : `kubectl logs [pod-name]`

### Exemple de Résumé

Si tu me fournis des sections spécifiques de la page GitHub, je pourrai te donner un résumé détaillé. En attendant, voici un exemple de résumé basé sur la structure typique ci-dessus :

---

### Kubernetes Cheat Sheet - Résumé

Ce cheat sheet Kubernetes fournit une référence rapide aux commandes kubectl et aux concepts essentiels pour gérer des clusters Kubernetes. Il couvre les aspects suivants :

1. **Commandes de Base** : Informations sur le cluster, gestion des ressources, création, suppression et application de configurations.
2. **Gestion des Pods** : Lister, décrire, consulter les logs et exécuter des commandes dans les pods.
3. **Services et Networking** : Lister, créer et décrire des services pour l'exposition des pods.
4. **Déploiements et Réplication** : Création, mise à jour et mise à l'échelle des déploiements.
5. **Volumes et Stockage** : Gestion des volumes persistants et des claims.
6. **Namespaces** : Gestion des namespaces pour l'isolation des ressources.
7. **Configurations et Secrets** : Création et gestion des ConfigMaps et Secrets.
8. **RBAC** : Gestion des rôles et des permissions.
9. **Debugging et Monitoring** : Outils et commandes pour le débogage et la surveillance des clusters.

---

N'hésite pas à me donner plus de détails ou des extraits spécifiques pour un résumé plus précis !

