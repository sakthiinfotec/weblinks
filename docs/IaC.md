#### Terraform

##### Advantages
* Multi-cloud
* Stateful
* Version controlled
* Declarative
* Scalable (Eg. count - To Spin off multiple instances)
* Saves Cost (Spin off the entire infrastructure when needed and Tear down when not in needed)
* Disaster Recovery
* Reduces Human Error

##### Lifecycle
* init
* validate
* plan
* apply
* destroy

##### Code Structure
* Main
* Variables
* Providers
* Output
* Modules
* State

##### Setup
# using aws access-key and secret-access-key
aws configure

terraform --help
terraform init
terraform plan
terraform verify

# format code
terraform fmt
terraform apply

# Following will override variables.tf
terraform apply -var "aws_instance_type=t2.micro" 

terraform destroy
