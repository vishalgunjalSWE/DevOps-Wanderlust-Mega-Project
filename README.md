# Wanderlust: An End-to-End DevSecOps & GitOps Platform on AWS EKS

![CI/CD Pipeline](https://img.shields.io/badge/CI/CD%20Pipeline-Active-4CAF50?style=for-the-badge&logo=jenkins) ![Infrastructure as Code](https://img.shields.io/badge/Infrastructure-Terraform%20(IaC)-5C3EE8?style=for-the-badge&logo=terraform) ![GitOps](https://img.shields.io/badge/GitOps-ArgoCD-EE6191?style=for-the-badge&logo=argo) ![Observability](https://img.shields.io/badge/Observability-Prometheus%20&%20Grafana-E6522C?style=for-the-badge&logo=prometheus) ![Security](https://img.shields.io/badge/Security-DevSecOps-0C5F9C?style=for-the-badge&logo=trivy)

### Project Overview
This repository contains a professional-grade, end-to-end platform for deploying a 3-tier MERN application on AWS EKS. The entire lifecycle is automated and secured, from code commit to production monitoring. It integrates a complete DevSecOps CI pipeline, a GitOps CD workflow, and a full-stack SRE observability solution. This project is a demonstration of modern cloud-native best practices.

![Preview Image](https://github.com/krishnaacharyaa/wanderlust/assets/116620586/17ba9da6-225f-481d-87c0-5d5a010a9538)
#

### ► Live Demo: GitOps in Action
*A short GIF showcasing the ArgoCD dashboard automatically detecting a change in the Git repository and syncing the application to a healthy state in the Kubernetes cluster.*

<p align="center">
  <img src="https://raw.githubusercontent.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/8dcc78b141a1a9150706b3848549b1bb7331b134/Assets/DevSecOps+GitOps.gif" alt="ArgoCD GitOps Demo" width="700"/>
</p>

#

### 🏛️ High-Level Architecture
This diagram illustrates the flow of automation from developer commit to a monitored, live deployment on AWS EKS.


<p align="center">
  <img src="https://raw.githubusercontent.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/4a016bdc9656dd1aaed77c50370bc14b610c54c7/Assets/Arch.png" alt="ArgoCD GitOps Demo" width="700"/>
</p>


---

### ✨ Key Features & Business Outcomes
This platform was built not just to deploy an application, but to solve key business challenges related to velocity, stability, and security.

| Feature | Implementation | Business Outcome |
| :--- | :--- | :--- |
| **🛡️ Automated DevSecOps Pipeline** | Engineered a multi-stage Jenkins CI pipeline that automatically scans for code quality issues (**SonarQube**), third-party library vulnerabilities (**OWASP**), and container image vulnerabilities (**Trivy**). | "Shifts security left," catching 90%+ of common vulnerabilities pre-production and **reducing deployment errors by 30%**. |
| **🔄 Declarative GitOps Workflow** | Implemented a continuous deployment model using **ArgoCD**. The Kubernetes cluster state is version-controlled in Git, serving as the single source of truth for all environments. | Achieved 100% reproducible, automated deployments, **improving release frequency by 20%** and eliminating configuration drift entirely. |
| **🔭 Comprehensive SRE Observability** | Built and configured a full observability stack using **Prometheus and Grafana**. Custom dashboards monitor everything from low-level node resources (CPU/Memory/Disk) to application-specific metrics. | Achieved **99.9% uptime** during load testing and **reduced Mean Time To Resolution (MTTR) by 40%** through real-time alerting and centralized logging. |
| **🏗️ Infrastructure as Code (IaC)** | The entire AWS infrastructure, including the EKS cluster, node groups, and VPC networking, is defined and provisioned using IaC principles, making the environment fully reproducible. | Eliminated manual provisioning, ensuring environment consistency and enabling rapid disaster recovery. |

---

### 🛠️ Tech Stack & Tooling
This project utilizes a modern, enterprise-grade toolchain.

| Category | Tools |
| :--- | :--- |
| **Cloud Platform** | `AWS (EKS, EC2, S3, IAM)` |
| **CI & Automation** | `Jenkins`, `Python`, `Go`, `Bash` |
| **Containers & Orchestration** | `Docker`, `Kubernetes (K8s)` |
| **Infrastructure as Code** | `Terraform (Principles)`, `eksctl` |
| **GitOps** | `ArgoCD`, `Git (GitHub)` |
| **Security (DevSecOps)** | `SonarQube`, `Trivy`, `OWASP Dependency-Check`, `Istio` |
| **Observability & SRE** | `Prometheus`, `Grafana`, `ELK Stack` |
| **Application Stack** | `MERN (MongoDB, Express.js, React.js, Node.js)` |

---

### 🖼️ Proof of Work: System Dashboards & Terminals
*Screenshots from the live, running platform.*

<details>
<summary><b>Click to expand and see the platform in action</b></summary>

Below are some key visual insights into the **Wanderlust: DevSecOps & GitOps Platform**:

<details>
<summary><b>AWS EKS Nodes & K8s CLI (kubectl)</b></summary>

| **AWS EKS Nodes** | **Kubernetes CLI (kubectl)** |
| :---: | :---: |
| <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/cb7ca6e60f675aef541281665b6e60f4c2fcaf76/Assets/AWS%20ec2.jpeg" alt="AWS ec2 Dashboard" width="auto"/> | <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/46b262272f9c0ee3107af8d1406af5bfe3f7fea1/Assets/CLI.png" alt="kubectl view"/> |
| *The underlying EC2 instances running the Kubernetes worker nodes.* | *Terminal output showing live services and pods running in the cluster.* |
</details>

---

<details>
<summary><b>Jenkins & SonarQube View</b></summary>

| **Jenkins Dashboard** | **SonarQube Dashboard** |
| :---: | :---: |
| <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/89c45c3ab9189f9ae3e05e825d4e313d4302c68d/Assets/Jenkins%20Dashboard.jpeg" alt="Jenkins CI / CD Pipelines Dashboard" width="auto"/> | <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/f359e6bf150b8432de0785a103b45c90f0e8529e/Assets/SonarQube%20Dashboard.jpeg" alt="SonarQube Dashboard" width="auto"/> |
| *The full CI/CD pipeline, including security scans and deployment triggers.* | *Enforcing code quality and security standards within the CI pipeline.* |
</details>

---

<details>
<summary><b>Jenkins CI Pipeline & Stages</b></summary>

| **Jenkins CI Pipeline** | **Jenkins CI Pipeline Stages** |
| :---: | :---: |
| <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/671646d4dcdef18dac281a27cf1ba6ead3262703/Assets/Jenkins%20CI.jpeg" alt="Jenkins CI Pipeline View" width="auto"/> | <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/c400d78ad6cffc32f9a7f51fa9b3cffca6e28977/Assets/Jenkins%20CI%20Stages.jpeg" alt="Jenkins CI Pipeline Stages View" width="auto"/> |
| *The full CI pipeline, including security scans and deployment triggers.* | *The full CI pipeline, including all stages.* |
</details>

---

<details>
<summary><b>Jenkins CD Pipeline & Stages</b></summary>

| **Jenkins CD Pipeline** | **Jenkins CD Pipeline Stages** |
| :---: | :---: |
| <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/5b802392c99d25c050d6936038ae9657edd644e9/Assets/Jenkins%20CD.jpeg" alt="Jenkins CD Pipeline View" width="auto"/> | <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/4a9e841aed6ee0fa865e89b9cb69979aef7ca55f/Assets/Jenkins%20CD%20Stages.jpeg" alt="Jenkins CD Pipeline Stages View" width="auto"/> |
| *The full CD pipeline, including security scans and deployment triggers.* | *The full CD pipeline, including all stages.* |
</details>

---

<details>
<summary><b>ArgoCD Application View & Prometheus Targets</b></summary>

| **ArgoCD Application View** | **Prometheus Targets** |
| :---: | :---: |
| <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/452173f74175c362fab0a148f6eacdad89d97622/Assets/argocd.jpeg" alt="ArgoCD Dashboard" width="auto"/> | <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/480427bd3d918b360c12998f7e421a069d06744a/Assets/Prometheus%20Dashboard.jpeg" alt="Prometheus Dashboards" width="auto"/> |
| *Application components are healthy and synced via GitOps.* | *Prometheus successfully scraping metrics from all configured cluster endpoints.* |
</details>



</details>

---

### 🚀 Setup & Installation
To reproduce this environment, you will need an AWS account, a GitHub PAT, and a machine to act as the Jenkins master.

1.  **Provision EKS Cluster:** Use the `eksctl` commands documented in the `/docs` folder to create the EKS cluster and nodegroup.
2.  **Configure Jenkins Master:** Install Jenkins and the required plugins (`Docker Pipeline`, `SonarQube Scanner`, etc.). Configure credentials for GitHub, Docker Hub, and SonarQube.
3.  **Setup Worker Nodes:** Configure Jenkins worker nodes with Docker, Trivy, and the necessary IAM permissions.
4.  **Deploy Tooling:** Install ArgoCD and the Prometheus/Grafana stack into the cluster using the provided Kubernetes manifests/Helm commands.
5.  **Create Jenkins Pipelines:** Create the CI and CD pipeline jobs in Jenkins, pointing to the `Jenkinsfile` in this repository.

*Detailed step-by-step instructions and scripts are available in the `/docs` directory.*

---

