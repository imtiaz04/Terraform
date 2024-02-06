using for_each command we can give names to the instances witch desired in that case terraform will destroy .tf file and create new instances
terraform {
   required_providers {
        aws = {
        source = "hashicorp/aws"
        version = "~> 4.16"

}
}

required_version = ">= 1.2.0"
}
provider "aws" {
region = "us-east-1"
}
locals {
        instance_name = toset(["sam","shyam","amar","akbar"])


}

resource "aws_instance" "aws_ec2_test" {
        for_each = local.instance_name
        ami = "ami-0c7217cdde317cfec"
        instance_type = "t2.micro"
        tags = {
 Name = each.key

}
}
~         
![image](https://github.com/imtiaz04/Terraform/assets/85178565/655d3cd9-9661-4fa7-9ea6-b93edcdaf60c)


![image](https://github.com/imtiaz04/Terraform/assets/85178565/c5411923-75ba-4e2b-93d4-24104d595655)



![image](https://github.com/imtiaz04/Terraform/assets/85178565/c0fa8361-8b32-47cb-90b3-ca55e996c473)




