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
* tfvars - contains key, value pairs and will override variables.tf

##### Setup
aws configure - using aws access-key and secret-access-key

terraform --help
terraform init
terraform plan
terraform verify

terraform fmt - format code
terraform apply

terraform apply -var "aws_instance_type=t2.micro" # Following will override variables.tf

terraform destroy

terraform output - to see output anytime

