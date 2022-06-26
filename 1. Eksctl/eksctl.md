Eksctl is an open source tool.  It is used to create and maintain EKS clusters on AWS and will configure the necessary infrastructure for our cluster. Also we can use eksctl to add new users to our cluster, add/remove worker nodes, enable logging through cloudwatch etc.

<hr>

Install eksctl
<br>
https://github.com/weaveworks/eksctl/releases/tag/v0.98.0
<img src="https://github.com/LawrenceDavy13/DevopsProject-3-Kubernetes/blob/main/images/1.%20Eksctl/image.png">
<img src="https://github.com/LawrenceDavy13/DevopsProject-3-Kubernetes/blob/main/images/1.%20Eksctl/image2.png">
<img src="https://github.com/LawrenceDavy13/DevopsProject-3-Kubernetes/blob/main/images/1.%20Eksctl/image3.png">

<br>

We need to provide a .yaml configuration file for EKS. I originally tried to use a t2.mirco for the instanceType to save on cost but the cluster refused to create properly. It seems like Kubernetes needs an ample amount of resources to function correctly.
<br>
<img src="https://github.com/LawrenceDavy13/DevopsProject-3-Kubernetes/blob/main/images/1.%20Eksctl/image4.png">
<br>
<img src="https://github.com/LawrenceDavy13/DevopsProject-3-Kubernetes/blob/main/images/1.%20Eksctl/image5.png">

<br>

Set environment variables. This create the cluster using our AWS credentials.
<br>
<img src="https://github.com/LawrenceDavy13/DevopsProject-3-Kubernetes/blob/main/images/1.%20Eksctl/image6.png">

<br>

Execute configuration file
<br>
<img src="https://github.com/LawrenceDavy13/DevopsProject-3-Kubernetes/blob/main/images/1.%20Eksctl/image7.png">
<img src="https://github.com/LawrenceDavy13/DevopsProject-3-Kubernetes/blob/main/images/1.%20Eksctl/image8.png">

<br>

It seems that kubectl is not included with the installation of eksctl. This is the error it got when creating the cluster and had to install kubectl separately.
<br>
<img src="https://github.com/LawrenceDavy13/DevopsProject-3-Kubernetes/blob/main/images/1.%20Eksctl/image9.png">
<img src="https://github.com/LawrenceDavy13/DevopsProject-3-Kubernetes/blob/main/images/1.%20Eksctl/image10.png">

<br>

View the worker nodes created. The master nodes are not showing because they are handled by AWS.
<img src="https://github.com/LawrenceDavy13/DevopsProject-3-Kubernetes/blob/main/images/1.%20Eksctl/image11.png">

<br>

Bonus: Delete cluster when finished.
<br>
<img src="https://github.com/LawrenceDavy13/DevopsProject-3-Kubernetes/blob/main/images/1.%20Eksctl/image12.png">








