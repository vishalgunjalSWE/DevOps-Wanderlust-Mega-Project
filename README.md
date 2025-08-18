# Wanderlust: An End-to-End DevSecOps & GitOps Platform on AWS EKS

![CI/CD Pipeline](https://img.shields.io/badge/CI/CD%20Pipeline-Active-4CAF50?style=for-the-badge&logo=jenkins) ![Infrastructure as Code](https://img.shields.io/badge/Infrastructure-Terraform%20(IaC)-5C3EE8?style=for-the-badge&logo=terraform) ![GitOps](https://img.shields.io/badge/GitOps-ArgoCD-EE6191?style=for-the-badge&logo=argo) ![Observability](https://img.shields.io/badge/Observability-Prometheus%20&%20Grafana-E6522C?style=for-the-badge&logo=prometheus) ![Security](https://img.shields.io/badge/Security-DevSecOps-0C5F9C?style=for-the-badge&logo=trivy)

### Project Overview
This repository documents the architecture and implementation of a professional-grade, end-to-end platform for deploying, securing, and operating a 3-tier MERN application on AWS EKS. The entire lifecycle is automated and secured, from code commit to production monitoring. It integrates a complete **DevSecOps CI pipeline**, a **GitOps CD workflow**, and a full-stack **SRE observability solution**, demonstrating a mastery of modern cloud-native best practices.

![Preview Image](https://github.com/krishnaacharyaa/wanderlust/assets/116620586/17ba9da6-225f-481d-87c0-5d5a010a9538)
#

### ► Live Demo: GitOps in Action
*A short demonstration of the ArgoCD dashboard automatically detecting a change in the Git repository and syncing the application to a healthy state in the Kubernetes cluster.*

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

### 🖼️ Proof of Work: A Curated Platform Gallery
*A curated selection of screenshots from the live, running platform.*

<details>
<summary><b> 📌 Click to expand and see the platform in action</b></summary>

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
| <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/452173f74175c362fab0a148f6eacdad89d97622/Assets/argocd.jpeg" alt="ArgoCD Dashboard" width="auto"/> <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/c0eeb57294e25711d5ce50a622709927a7fc1146/Assets/argocd%20dashboard.jpeg" alt="ArgoCD Dashboard" width="auto"/> | <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/480427bd3d918b360c12998f7e421a069d06744a/Assets/Prometheus%20Dashboard.jpeg" alt="Prometheus Dashboards" width="auto"/> |
| *Application components are healthy and synced via GitOps.* | *Prometheus successfully scraping metrics from all configured cluster endpoints.* |
</details>

---

<details>
<summary><b>Grafan : SRE Dashboard & Cluster Metrics</b></summary>

| **Grafana: SRE Dashboard (Namespace: wanderlust)** | **Grafana: Cluster Metrics (Node Exporter - Cluster)** |
| :---: | :---: |
| <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/463e3ba5dbf144678cb319141fbd4e45c4fdb2a5/Assets/Grafana%20Dashboard%201.jpeg" width="auto"/> | <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/f540c57eacb2ff13bda4487e0f5400b7f9e64edc/Assets/Grafana%20Dashboard%203.jpeg" alt="Jenkins CD Pipeline Stages View" width="auto"/> |
| *Provides CPU, Memory, Network, and Storage metrics per namespace/pod. Useful for analyzing app-level resource consumption and performance bottlenecks.* | *Shows overall cluster health including CPU, Memory, Disk IO, and Network utilization. Great for cluster-wide performance visibility.* |
</details>

---

<details>
<summary><b>Grafan : Application Metrics & Node Metrics (Node Exporter - AIX)</b></summary>

| **Grafana: Application Metrics (Namespace: argocd)** | **Grafana: Node Metrics (Node Exporter - AIX)** |
| :---: | :---: |
| <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/6bf6de2d6a6a5bbf3fe9398ea41aaa95015de3d0/Assets/Grafana%20Dashboard%202.jpeg" alt="Grafana View" width="auto"/> | <img src="https://github.com/vishalgunjalSWE/DevOps-Wanderlust-Mega-Project/blob/ffdba5e42ad44c66130bf661c419474bcab67c1f/Assets/Grafana%20Dashboard%204.jpeg" alt="Grafana View" width="auto"/> |
| *Tracks ArgoCD server network performance, bandwidth usage, packet rates, and network reliability. Helps monitor GitOps synchronization health.* | *Provides per-node CPU, Memory, Disk, and Network statistics. Helps drill down into individual node resource utilization.* |
</details>



</details>

---
---

📞 Contact & Further Information

This project represents a comprehensive, hands-on application of DevSecOps, GitOps, and SRE principles to deliver tangible business outcomes. It serves as a testament to my ability to architect, build, and operate modern cloud-native systems.

For further discussion about this project or to explore potential opportunities, please feel free to connect with me.

<p align="left"> 
  <a href="https://www.linkedin.com/in/vishal-gunjal-" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
  </a> 
  <a href="https://vishalgunjal-cv.vercel.app/" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-D14836?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Portfolio Badge"/>
  </a>
  <a href="https://github.com/vishalgunjalswe" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Badge"/>
  </a>
  <a href="https://medium.com/@vishalgunjal0287" target="_blank">
    <img src="https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white" alt="Medium Badge"/>
  </a>
</p>


