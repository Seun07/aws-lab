# command to copy files into s3 bucket
aws s3 cp secret s3://<bucket name> --recursive
aws sts get-caller-identity
aws s3 rm s3://sheck-bucket --recursive 
aws s3 cp s3://sheck-bucket receiver --recursive 
