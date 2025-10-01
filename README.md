# Terraform
- Infra provisioning tool (cloud provider agnostic) , converts files to native APIs of the cloud provider that we select. (IAC tools like cloud formation templates, heatmaps, azure resource manager are cloud provider specific)
- Authenticating with the providers
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
- tree command useful
- ssh -i key ubuntu@ip_address command to ssh into ec2 instance, listing useful commands for devops engineers
- ssh-keygen -t rsa, creates a public and a pvt key in the folder ~/.ssh/id_rsa
- Best practices to manage statefile
- scenario based questions practice
- syntax practice
- Study how to implement different deployment types using terraform (blue-green, canary)
- Terraform with CI/CD pipeline
- Terraform project template (key directories and files and their significance)
- terraform built in functions like depends_on (a resource should be created before the other resource), count(number of resources to be created), map (std cpp type map)
- Automated testing for terraform code using terratest, kitchen-terraform, tflint etc

# CI/CD
- Github actions
- Jenkins

# Ansible

# Docker

# Kubernetes

# Cloud providers
- AWS
- Azure
- GCP

# Networking 
# Linux
