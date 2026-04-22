Summary & Key Takeaways 
The deployment leveraged a wide range of AWS services to architect a scalable, secure, 
and highly available cloud environment. The solution centered on Kubernetes 
orchestration, containerization, and robust networking to support modern application 
needs. Amazon EKS was used to manage the Kubernetes control plane, while worker 
nodes handled application workloads across private subnets

AWS Services Covered 
• VPC (Virtual Private Cloud) – Custom network configuration and isolation 
• Subnets (Public & Private) – Tiered design for application, worker node, and 
database separation 
• Internet Gateway (IGW) – Enabled inbound/outbound traffic for public subnets 
• NAT Gateway – Allowed private subnets to access the internet securely 
• Route Tables – Directed public and private traffic paths 
• Security Groups – Controlled inbound and outbound access between layers 
• EC2 Instance Connect Endpoint (EICE) – Provided secure SSH access to private 
EC2 instances without bastion hosts 
• Amazon S3 – Stored application code for centralized access during deployment 
• IAM Users & Roles – Enabled programmatic access, service-to-service 
permissions, and EKS cluster/worker node authorization 
• RDS (Relational Database Service) – Managed MySQL database with subnet 
groups in private subnets 
• Secrets Manager – Stored and retrieved sensitive database credentials and GitHub 
tokens securely 
• Amazon ECR (Elastic Container Registry) – Stored private Docker images for 
Kubernetes deployments 
• Amazon EKS (Elastic Kubernetes Service) – Managed Kubernetes control plane for 
container orchestration 
• EKS Worker Nodes – EC2 instances running Kubernetes pods to serve application 
workloads 
• EKS Cluster IAM Roles – Authorized the EKS control plane and worker nodes to 
interact with AWS services 
• Kubernetes Service (LoadBalancer) – Exposed the application to external traffic 
via an AWS load balancer 
• Route 53 – Managed DNS and domain routing for public access to the application 
• AWS Certificate Manager (ACM) – Issued and managed SSL/TLS certificates for 
secure HTTPS connections 
Containerization, Kubernetes & DevOps Tools 
• Docker – Containerized the web application for consistency across environments 
• Dockerfile – Defined application dependencies and runtime configuration 
• Kubernetes (kubectl) – Managed cluster resources, deployments, and services via 
the command line 
• eksctl – Simplified EKS cluster creation and worker node provisioning 
• Helm – Kubernetes package manager for managing application deployments 
• Kubernetes Manifest Files – Declared desired state for deployments, services, and 
other cluster resources 
• Git – Distributed version control system for tracking code changes and 
collaboration 
• GitHub – Version-controlled application code, Dockerfiles, and Kubernetes 
configurations 
• AWS CLI – Automated resource creation and deployment workflows 
