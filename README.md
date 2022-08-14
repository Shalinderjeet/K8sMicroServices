Project Title:- Deploy Microservices application in Kubernetes with Production & Security Best Practices in Linode Cluster

Description:- Create K8s manifests for Deployments and Services for all microservices of an onlineshop application.
               Deploy microservices to Linode’s managed Kubernetes cluster.
               
               
-----------------------------------------------------------------------------------------------------------------------------------------------------
Online Boutique is a cloud-native microservices demo application. Online Boutique consists of a 10-tier microservices application. The application is a web-based e-commerce app where users can browse items, add them to the cart, and purchase them.

https://github.com/Shalinderjeet/microservices-demo

-----------------------------------------------------------------------------------------------------------------------------------------------------
Configure config.yaml with 11 microservices (deployments) with their corresponding 10 internal and 1 external service.

------------------------------------------------------------------------------------------------------------------------------------------------------
Create a K8s cluster on Linode and deploy your microservices on Linode K8s Cluster (LKE).
Download kube-config.yaml file to connect to the Linode K8s cluster.
Set the stricter permissions on kubeconfig.yaml file i.e chmod 600 kubeconfig.yaml
export KUBECONFIG=kubeconfig.yaml
kubectl get nodes
kubectl create namespace microservices
kubectl apply -f config.yaml -n microservices

kubectl get pod -n microservices
kubectl get service -n microservice

Access the application from any IPnode:30007
