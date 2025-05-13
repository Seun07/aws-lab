# command to copy files into s3 bucket 
aws s3 cp secret s3://<bucket name> --recursive 
aws sts get-caller-identity 
aws s3 rm s3://sheck-bucket --recursive
aws s3 cp s3://sheck-bucket receiver --recursive
aws s3 ls
aws s3 mv seun s3://sheck-bucket --recursive
# Cmd to create bucket using aws cli
aws s3 mb s3://aws-lagos2000 --region eu-north-1
# First delete all the objects present in given a bucket
aws s3 rm s3://gfg-example --recursive
# Cmd to remove bucket
aws s3 rb s3://aws-lagos1 --region eu-north-1
============================================
AWS Cli command for IAM 
============================================
# Cmd to create IAM user
 aws iam create-user --user-name jack
# cmd to list IAM users
aws iam list-users
# cmd to delete the IAM user
aws iam delete-user --user-name jack
============================================
AWS Cli Command to work on key pair 
============================================
# cmd to create key pair 
aws ec2 create-key-pair --key-name sandal
# cmd to delete key pair 
aws ec2 delete-key-pair --key-name sandal2
# AWS Cli command for creating Security Group
aws ec2 describe-security-groups --group-ids sg-07d609f75ec60c6c3
aws ec2 create-security-group --group-name MySecurityGroup --description "My security group"
# AWS Cli command for creating Security Group
aws ec2 create-security-group --group-name Onyabo --description "My security group"
# Delete ec2 security group
aws ec2 delete-security-group   --group-id sg-07d609f75ec60c6c3
# Create ec2 instance
aws ec2 run-instances --image-id <ami-id> --count 1 --instance-type t2.micro   --key-name <Keypair-name> --security-group-ids <SecurityGroupId> 
--subnet-id <SubnetId>
aws ec2 run-instances --image-id ami-0dd574ef87b79ac6c --count 1 --instance-type t2.micro --key-name sandal --security-group-ids 01274115d5c2adf5b --subnet-id 04db98a792830478c
# describe an ec2 instance using cli
aws ec2 describe-instances --instance-ids i-024bc6b349451521c
# to stop an ec2 instance using cli
aws ec2 stop-instances --instance-ids i-024bc6b349451521c
# to terminate or delete an ec2 instance
aws ec2 terminate-instances --instance-ids i-1234567890abcdef0

i-0e08786073f874a5e