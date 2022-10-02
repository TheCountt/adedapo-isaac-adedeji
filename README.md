# Implementation of an Integrated Infrastructure

To implement the infrastructure,a cloud managed kubernetes service(Elastic  Kubernetes Service) was provisioned on the cloud service provider(AWS) with an Infrastructure as Code tool called Terraform.

**Note**: A configuration tool called Ansible was used to install and configure neccessary packages, CLI tools and softwares that will be needed by the Kubernetes cluster to work properly on workstation (Bastion server) that was spun up on cloud(AWS) 

## Pre-requisite Knowledge
- Knowledge of cloud service provider (AWS, Azure, GCP,etc)
- Proficience in Terraform (Infrastructure Provision)
- Proficience in Ansible (Configuration Management)
- Knowledge of Docker (Containerization)
- Knowledge of Kubernetes (Container Orchestration)
- Knowledge of Helm (Package Manager for Kubernetes)

## Incorporated Technologies include:
- Grafana and Prometheus (Monitoring)
- Apisix (Security)
- Dapr (Configuration)
- yugabyteDB (Data Management Storage)
- Kubeflow (Data Science and AI)
- Docker (Application)
- Kafka (Communication)
- Superset (Visualization)


## Steps

- Install and configure Ansible version 2.10 or above on workstation (Use Ansible documentation)

- Write ansible scripts to install and configure other necessary softwares, dependencies and CLI tools on workstation (Check ansible scripts for reference)

*Note*: Structure ansible folders and files to accommodate code expansion and for easy understanding upon inheritance

- Run ansible playbook file against the inventory file

- A file was created to house the terraform scripts

- Programmatic access to AWS was given to the workstation so resources can be created in AWS by Terraform 

- A Kubernetes cluster was provisioned using Terraform

- Helm CLI was then used to deploy the desired technologies.

**Note**:

        - Kubernetes packages specified in the documentation of the technologies and Artifact Hub(A web-based application that enables finding, installing, and publishing Kubernetes packages) were the helm charts repositories used

        - Neccessary ports of the technologies deployed were opened on the workstation to be able  to route traffic.










