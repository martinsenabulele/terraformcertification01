iiiii### Important Note

Note that every region has a different AMI ID. The AMI ID's keeps on changing so make sure you use the latest AMI ID from the AWS console similar to the way it is shown in the video.

### first_ec2.tf

```sh
provider "aws" {
  region     = "us-west-1"
  access_key = "AKIAILAR7KDR7X7HTXLQ"
  secret_key = "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"
}

resource "aws_instance" "myec2" {
   ami = "ami-04d29b6f966df1537"
   instance_type = "t2.micro"
}
```
### Commands:

```sh
terraform init
terraform plan
terraform apply
```
