# Commands to execute:
*OBS: the flag **"-var-file"** it's for the stored variables in a file*
* Initiate directory for Terraform:
```
terraform init -var-file=openstack_variables.tfvars
```
* Validate configurations files (*.tf) in the current directory:
```
terraform validate
```
* Plan the code to execute:
```
terraform plan -var-file=openstack_variables.tfvars
```
* Execute the code:
```
terraform apply -auto-approve -var-file=openstack_variables.tfvars
```
* Undo everything you did in the command "apply"
```
terraform destroy -auto-approve -var-file=openstack_variables.tfvars
```