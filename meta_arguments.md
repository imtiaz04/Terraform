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
resource "aws_instance" "aws_ec2_test" {
        count = 4
        ami = "ami-0c7217cdde317cfec"
        instance_type = "t2.micro"
        tags = {
 Name = "TerraformTestServer-${count.index}"

}
}
here count is meta argument which will create instances with indexing
![image](https://github.com/imtiaz04/Terraform/assets/85178565/6f42abd1-c39d-46d8-b490-d77baac0e522)

![image](https://github.com/imtiaz04/Terraform/assets/85178565/b798139d-6886-4e4c-89a2-59902d2a2c00)

