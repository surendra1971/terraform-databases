# terraform-databases

This is the root module which calls all the 4 databases, all the databases that will be created in future will be called from here.


### terraform commands with backend config in a environment specific file 

```
   terrafile -f env-dev/Terrafile
 $ terraform init -backend-config=env-dev/dev-backend.tfvars
 $ terraform plan -var-file=env-dev/dev.tfvars
 $ terraform apply -auto-approve -var-file=env-dev/dev.tfvars
 terraform destroy -auto-approve -var-file=env-dev/dev.tfvars
```