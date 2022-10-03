# Implementation of an Integrated Infrastructure

To implement the infrastructure,a cloud managed kubernetes service(Elastic  Kubernetes Service) was provisioned on the cloud service provider(AWS) with an Infrastructure as Code tool called Terraform.

**Note**: A configuration tool called Ansible was used to install and configure neccessary packages, CLI tools and softwares that will be needed by the Kubernetes cluster to work properly on the workstation (Bastion server) that was spun up on cloud(AWS) 

## Pre-requisite Knowledge
- Knowledge of cloud service providers (AWS, Azure, GCP,etc)
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



<img width="658" alt="Screenshot 2022-10-02 215009" src="https://user-images.githubusercontent.com/76074379/193512762-c33bff65-72f7-4a5e-9bf2-17a201657346.png">


<img width="786" alt="Screenshot 2022-10-02 215041" src="https://user-images.githubusercontent.com/76074379/193512856-393657aa-d6a7-4cb9-9159-92bb4732e355.png">

<img width="753" alt="Screenshot 2022-10-02 215115" src="https://user-images.githubusercontent.com/76074379/193512917-5c864dbb-d34c-4126-8ac6-57180c6ef2b2.png">

<img width="587" alt="Screenshot 2022-10-02 215138" src="https://user-images.githubusercontent.com/76074379/193512978-5ebea171-1c8b-4be8-8d9d-b5a42aa1a208.png">








