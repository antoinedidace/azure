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
```
