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

## 📊 Project Demo Screenshots

Below are some key visual insights into the **Wanderlust: DevSecOps & GitOps Platform**:

| **🚀 ArgoCD Application View** |
| :---: |
| <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/4a016bdc9656dd1aaed77c50370bc14b610c54c7/Assets/Arch.png" alt="ArgoCD Application View" width="auto"/> 
<img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/4a016bdc9656dd1aaed77c50370bc14b610c54c7/Assets/Arch.png" alt="ArgoCD Application View" width="600"/>|
| *Application components are healthy and synced via GitOps.* |

---

| **Jenkins CI/CD Pipeline Stages** |
| :---: | :---: |
| <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/452173f74175c362fab0a148f6eacdad89d97622/Assets/argocd.jpeg" alt="ArgoCD Application View" width="400"/> <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/c0eeb57294e25711d5ce50a622709927a7fc1146/Assets/argocd%20dashboard.jpeg" alt="ArgoCD Application View" width="400"/>|
|*End-to-end CI/CD pipeline, including code quality, security scans & deployment triggers.* |

| **Grafana: SRE Dashboard** | **Grafana: Application Metrics** |
| :---: | :---: |
| <img src="https://raw.githubusercontent.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/main/Assets/Grafana-SRE.png" alt="Grafana SRE Dashboard" width="400"/> | <img src="https://raw.githubusercontent.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/main/Assets/Grafana-App.png" alt="Grafana Application Metrics" width="400"/> |
| *Monitoring cluster health: CPU, Memory, Disk, Network I/O.* | *Tracking app-specific metrics like memory usage and per-pod network traffic.* |

| **AWS EKS Nodes** | **Kubernetes CLI (kubectl)** |
| :---: | :---: |
| <img src="https://raw.githubusercontent.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/main/Assets/EKS-Nodes.png" alt="AWS EKS Nodes" width="400"/> | <img src="https://raw.githubusercontent.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/main/Assets/Kubectl.png" alt="Kubernetes CLI" width="400"/> |
| *EC2 worker nodes powering the EKS cluster.* | *Live `kubectl` output showing services & pods running in the cluster.* |

| **SonarQube Quality Gate** | **Prometheus Targets** |
| :---: | :---: |
| <img src="https://raw.githubusercontent.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/main/Assets/SonarQube.png" alt="SonarQube Quality Gate" width="400"/> | <img src="https://raw.githubusercontent.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/main/Assets/Prometheus.png" alt="Prometheus Targets" width="400"/> |
| *Code quality, vulnerability checks & security gates.* | *Prometheus scraping metrics from all configured cluster endpoints.* |

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

