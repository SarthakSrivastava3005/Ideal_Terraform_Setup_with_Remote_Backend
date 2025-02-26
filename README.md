🔄 Order of Running the Script:

1️⃣ Configure AWS CLI: Ensure your AWS CLI is set up correctly with proper credentials.

2️⃣ Remote State Setup:

 • Navigate to the aws/remote_state/ directory in your terminal and execute the main.tf file.

 • This creates remote backend resources—an S3 bucket and a DynamoDB table—for state storage and locking.

3️⃣ Local State Configuration:

 • Then, navigate to the aws/local_state/ directory and execute the main.tf file, which configures the backend for your EC2 instance creation.

 • Once executed, check the AWS Console to confirm that the S3 bucket (holding the state file) and DynamoDB table are created in the specified region.
