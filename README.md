# DevopsProject-3

In this project I wanted to try a deeper dive into the world Kubernetes, since it is alot more popular than Cloudformation, is cross-platform and I just wanted a challenge using microservices. Well thats exactly what I got. 
<br>
So first, I tried to building my Kubernetes cluster from scratch. The Ansible and Packer configuration was straight forward, although the Terraform part was challenging. This is then I realised why most companies decide to let their cloud providers handle their clusters. The amount of setup that Kubernetes requires by Terraform, for creating non-EKS clusters and for setting Gitlab CI is huge and since this was my first project involving Terraform, I got to lost in the weeds and honestly didn't know what I was doing.
<br>
In the end, I ended up using Eksctl to create and manage the clusters. What took hours of setup, now only took 20 minutes or so and with that, I managed to complete the pipeline for this project.
<br>
As much head banging as their was in creating this project, it was fun and appreciated how powerful Kubernetes.
<br>
I do plan to create an alternative project, with the setup involving Terraform and using either Kustomize or Kubernetes Operators for provisioning the application. Since I don't plan on giving up on the progress I made during my first attempt. 
<br>
BONUS: Will update this project adding Velero disater recovery tool.


Tools included:

- OS - Ubuntu 22.04 - WSL2 Windows 10
- Git - Local version control system
- Gitlab - Continuous integration tool
- Docker - Containerization
- Kubernetes - Container management
- Helm - Kubernetes package management
- AWS - Cloud
