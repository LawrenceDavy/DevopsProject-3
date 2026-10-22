# DevOps Project 3 — EKS, Helm and CI/CD Lab

In this project I explored deploying a containerised application to Kubernetes on AWS and connecting the deployment steps into a CI/CD workflow.

My original plan involved building more of the Kubernetes infrastructure using Terraform. I found that approach too complicated for this stage of learning, so I changed to **eksctl** to provision the EKS cluster and continued with Helm and GitLab CI/CD. I documented this change because it was part of the learning process.

**Status:** Historical hands-on project. These notes have not been re-tested against current AWS, EKS or GitLab versions; they should not be treated as a production-ready deployment.

## Tools used

AWS EKS, eksctl, Docker, Kubernetes, Helm, GitLab CI/CD and Ubuntu/WSL2.

## Project sections

- [EKS cluster setup with eksctl](1.%20Eksctl/)
- [Helm](2.%20Helm/)
- [CI/CD workflow and deployment notes](3.%20CICD/)

## What I learned

- The difference between assembling a cluster from many individual components and using a managed cloud service
- How container images, Helm charts and a CI/CD pipeline fit into deployment
- Why a working learning environment is not automatically a secure, repeatable production environment

## Limitations

- Some steps depend on old cloud/tool versions or resources that may no longer exist.
- There is no claim that this can be deployed unchanged today.
- I would add version pinning, secret handling, more deployment validation and recovery testing before using this approach in a real environment.

I kept the original project notes and structure so the decisions, challenges and progress remain visible.
