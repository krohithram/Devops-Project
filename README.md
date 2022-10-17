### AWS Cloud for Web App Setup
# Flow of Execution
- Login to AWS Account
- Create Key Pairs
- Create Security Groups
- Launch Backend EC2 Instances with User Data (Bash Scripts)
- Update IP to name Mapping in Route 53.
- Launch Tomcat EC2 Instance.
- Build Application from Source Code in local machine.
- Create IAM user (krr-s3-admin) Programatic access with AmazonS3FullAccess.
- Upload Artifact to S3 bucket
- Create a role to Download Articat into EC2 instance. 
- Download artifact to Tomcat EC2 Instance.
- Setup ELB with HTTPS 
- Create CName Record point ELB endpoint to name in Godaddy DNS.
- Verify Access url
- Build AMI & Auto Scaling group for Tomcat Instances.




