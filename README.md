# infrastructure

NUID: 001523415
Name: Vaishnavi Kiran Khismatrao

AWS VPC using Cloudformation

1)Create Virtual Private Cloud (VPC)
2)Create subnets (Links to an external site.) in your VPC. You must create 3 subnets, each in a different availability zone in the same region in the same VPC.
3)Create an Internet Gateway (Links to an external site.) resource and attach the Internet Gateway to the VPC.
4)Create a public route table (Links to an external site.). Attach all subnets created to the route table.
5)Create a public route in the public route table created above with destination CIDR block 0.0.0.0/0 and internet gateway created above as the target.
6)Create security groups for SSH

Commands to run the yaml file:-

aws cloudformation create-stack --stack-name VPCstack --template-body file://csye6225-infra.yaml

command to delete the stack:-

aws cloudformation delete-stack --stack-name VPCstack