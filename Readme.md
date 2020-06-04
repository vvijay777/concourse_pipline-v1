# Concoure Pipeline Sample

**Pre requisite**

	Install Concourse 
	Install Fly 
	Install Docker 
	AWS Access

```

Copy the script and pass the required AWS credentials in the below format. This will perform the below tasks 
	1) Get the Terraform enabled Docker Image
	2) Check the Terraform Version
	3) Plan / Apply terraform and create the AWS Resource (Dynamo DB)
	4) Remove the terraform created resource

Note: Please specify the aws bucket name & credentials according to your account 

fly -t ps set-pipeline -c terraform-pipeline.yml -p terraform-pipeline-v1 -v access-key=XXXX -v secret-key=XXXX

```
