#This template creates an S3 bucket and sets up a CloudFront distribution to serve files from the bucket.

#Code steps:
# 1) Create an S3 bucket with security configurations (encryption, versioning, public access blocked)
# 2) Create Origin Access Control (OAC) for secure CloudFront-S3 integration
# 3) Create a CloudFront distribution with S3 as origin
# 4) Configure CloudFront distribution settings (caching, HTTPS redirect, compression)
# 5) Create an S3 bucket policy to allow CloudFront access via OAC
# 6) Output important URLs and resource identifiers for easy access

# 1. Deploy CloudFormation stack → Wait for "CREATE_COMPLETE"
# 2. Upload files to S3 bucket
# 3. Access via CloudFront URL (Distribution domain name)

#Deployment Steps:
# 1) Go to AWS Management Console 
# 2) Navigate to CloudFormation
# 3) Click on "Create Stack" and choose "With new resources (standard)"
# 4) Choose "Upload a template file" or "Specify an Amazon S3 template URL" or Sync to GitHub
# 5) Upload your YAML file and click next 
# 6) Enter the stack name and parameters
# 7) Review the settings and click "Create stack"
# 8) Wait for the stack creation to complete
# 9) Once the stack is created, you can check the resources created in the CloudFormation console
# 10) You can check the S3 bucket and CloudFront distribution created in the respective consoles
# 11) Manually upload your files to the S3 bucket via AWS Console or CLI

