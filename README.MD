# Amazon EKS Cluster with Terraform
 
This repository contains Terraform code to deploy a fully functional Amazon EKS cluster with worker nodes, IAM roles, and VPC networking.
 
## Features
- Creates a secure VPC with subnets for the EKS cluster.
- Provisions an EKS cluster and node group.
- Configures IAM roles and policies.
- Outputs cluster endpoint and authentication certificate.
 
## Prerequisites
- AWS CLI configured with appropriate permissions.
- kubectl installed.
 
## Deployment Steps
 
1. Clone the repository:
   
   https://github.com/Jayakrishna7478/k8-eksctl.git

2. run aws congigure by provider aws IAM AWS Access kye and AWS Secret key Acredentials
   aws configure

3. cd k8-eksctl/

 eksctl create cluster --config-file=eks.yaml

4. install helm chart

$ curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
$ chmod 700 get_helm.sh
$ ./get_helm.sh

5. deploy helmchart blow command 
   helm install