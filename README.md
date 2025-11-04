# 🚀 DevOps 2025 — Practical Infrastructure Automation Lab

Welcome to **DevOps 2025**, a hands-on environment for practicing real-world DevOps workflows, automation, and CI/CD pipeline design.  
This repository showcases examples of how to build, configure, and deploy modern cloud-native infrastructure using industry-standard tools.

---

## 🧰 Tech Stack

| Tool | Purpose |
|------|----------|
| **Terraform** | Infrastructure as Code (IaC) — provisioning AWS EC2, networking, and K3s clusters |
| **Ansible** | Configuration management and server automation |
| **Docker / Docker Compose** | Containerization and local environment setup |
| **K3s (Lightweight Kubernetes)** | Orchestration for containerized workloads |
| **Helm** | Application deployment management |
| **Jenkins** | Continuous Integration / Continuous Deployment (CI/CD) |
| **GitHub Actions** | Optional lightweight CI/CD for testing automation |
| **Prometheus / Grafana** | Monitoring and observability setup |

---

## 🧱 Project Structure

devops-2025/
├── ansible/
├── terraform/
├── jenkins/
├── k3s/
├── docker/
├── scripts/
└── README.md


---

## 🧪 Usage

### 1️⃣ Clone the repository
```bash
git clone git@github.com:ilhomJohn81/devops-2025.git
cd devops-2025
2️⃣ Initialize Terraform
cd terraform
terraform init
terraform apply -auto-approve

3️⃣ Configure with Ansible
cd ../ansible
ansible-playbook site.yml -i inventory/aws.ini

4️⃣ Deploy workloads to K3s
cd ../k3s
helm install demo ./chart

🧩 Jenkins Pipeline Example
pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'docker build -t devops2025-app .'
      }
    }
    stage('Deploy') {
      steps {
        sh 'ansible-playbook playbooks/deploy.yml'
      }
    }
  }
}

📊 Observability

The project integrates Prometheus + Grafana to monitor system metrics and visualize CI/CD efficiency.

🧠 Learning Goals

Practice Infrastructure as Code (IaC) with Terraform

Automate configuration management using Ansible

Build and deploy workloads using Kubernetes / K3s

Understand CI/CD principles using Jenkins pipelines

Learn how to monitor and secure DevOps environments

👨‍💻 Author

Ilhom (ilhomJohn81)
DevOps Engineer | Cloud Infrastructure Enthusiast | Open Source Contributor