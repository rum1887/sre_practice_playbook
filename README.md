# SRE Playbook

# Terraform
- Infra provisioning tool (cloud provider agnostic) , converts files to native APIs of the cloud provider that we select. (IAC tools like cloud formation templates, heatmaps, azure resource manager are cloud provider specific)
- IDE and plugins setup (VSCODE)
- Authenticating with the providers (aws configure command for ex)
- Main commands (Lifecycle of terraform)
  - terraform init
  - terraform plan
  - terraform apply
  - terraform destroy
  - terraform import (to import statefile config for a resource manually created on a cloud provider (code must be written first before import))
  - terraform workspace -h (terraform workspace new dev; terraform workspace select dev;) (to manage multiple env with single terraform project; multiple statefiles for each env)
- Creating Terraform modules
- Configuring remote backends and applying locks to handle concurrent "terraform apply" requests
- Provisioners for ansible like capablities (local-exec, remote-exec)
- Secrets management (hashicorp vault)
- tree command useful (had to brew install because it was not present by default)
- ssh -i key ubuntu@ip_address command to ssh into ec2 instance, listing useful commands for devops engineers
- ssh-keygen -t rsa, creates a public and a pvt key in the folder ~/.ssh/id_rsa
- Best practices to manage statefile
- Scenario based questions practice
- Syntax practice
- Study how to implement different deployment types using terraform (blue-green, canary)
- Terraform with CI/CD pipeline
- Terraform project template (key directories and files and their significance)
- Terraform built in functions like depends_on (a resource should be created before the other resource), count(number of resources to be created), map (std cpp type map)
- Automated testing for terraform code using terratest, kitchen-terraform, tflint etc

# CI/CD
- Github actions
- Jenkins

# Ansible
- To create resources on remote servers
- Idempotent (resources already created will not be recreated)
- password less authentication?
- ansible adhoc cammands
- ansible playbooks (scripts to manage)
- ansible roles (directory structure templates)
- ansible collections to provision resources using api. Host? local host
- ansible vault
- practice exercises

# Docker

# Kubernetes

# Cloud providers
- AWS
    - Public vs private cloud
    - EC2 instances (elastic cloud compute, compute optmized, memory optimized, storage optmized etc)
    - S3 buckets (simple storage service, upto 5tb of data)
    - VPC (Virtual private cloud)
    - Load balancer (Healthchecks and sends requests to appropriete server)
    - Route53 DNS Service (helps resolve domain name)
    - Jump servers (Let's you connect to pvt subnets)
    - NAT Gateways (Lets pvt subnets connect to the internet, hides the IP of the pvt subnet, instead uses its own IP)
    - Subnets (Number of IPs/ range of IPs)
    - Autoscaling groups (helps scale resources during high traffic)
    - Route tables (helps route traffic)
    - Security groups (allow/deny traffic at instance level)
    - NACLs (Network access control list: denys traffic at a subnet level)
    - 
- Azure
    - Azure devops and security services
    - Azure git, Azure boards, Azure pipelines, Azure repositories
    - Sentinal, Log analytics workspace, Logic apps  
- GCP

# Networking 

# Linux
chown ownwe_name:group_name filename
chmod 600(rw-) filename

# Observablity tools 
- Grafana
- Prometheus

# Handy python scripts
# Version control
