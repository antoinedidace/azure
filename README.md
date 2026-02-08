# Microsoft Azure utility


## Build Azure image using Packer
```bash
# Switch to Azure utility directory.
$ cd <PROJECT_ROOT_DIR>
$ cd /opt/source/devel/slst/my-cloud-project

# Initialize Packer module.
$ packer init azure/image/alma-linux-9.pkr.hcl

# Validate Packer module.
$ packer validate azure/image/alma-linux-9.pkr.hcl

# Build VM image using Packer module.
$ packer build azure/image/alma-linux-9.pkr.hcl

## Build Kubernetes cluster in Azure using Azure Resource Manager (ARM)
```bash
# Switch to Azure utility directory.
$ cd <PROJECT_ROOT_DIR>
$ cd /opt/source/devel/slst/my-cloud-project/azure/arm

# Create Azure Kubernetes cluster.
$ az deployment group create -g sloopstash-prd -f arm/deployment/kubernetes.json
```
