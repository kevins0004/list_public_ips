# list_public_ips


# Required Software

# Python: 
The script is written in Python, so you need Python installed on your machine. Python 3.x is recommended for better compatibility with newer libraries.

# AWS CLI: 
The AWS Command Line Interface is used to configure your AWS credentials, which the script uses to access your AWS account.

# Boto3: 
This is the Amazon Web Services (AWS) SDK for Python. It allows Python developers to write software that makes use of services like Amazon S3 and EC2.
A Text Editor: Any text editor (like VS Code, Sublime Text, or even a basic one like Notepad) for editing the Python script.


# Steps to Set Up and Run the Script

# Install Python:

Download and install Python from python.org.
Ensure Python is added to your system's PATH variable during installation.

# Install AWS CLI:

Download and install the AWS CLI from AWS's official site.
Configure the AWS CLI by running aws configure in your command line. Enter your AWS Access Key, Secret Key, default region, and output format as prompted.

# Install Boto3:

Open a command line or terminal and install Boto3 using pip (Python’s package manager) by running pip install boto3.
Set Up AWS Credentials:

Your AWS credentials (Access Key ID and Secret Access Key) should be stored in a file at /home/ejev/.aws/credentials (assuming a Unix-like system). The file should look like this:

[default]
aws_access_key_id = YOUR_ACCESS_KEY_ID
aws_secret_access_key = YOUR_SECRET_ACCESS_KEY

# Write the Python Script:

Using a text editor, write or paste the Python script provided earlier. Save it with a .py extension, such as list_public_ips.py.
Run the Script:

Open your command line or terminal.
Navigate to the directory where your script is saved using the cd command.
Run the script by typing python list_public_ips.py.
The script will generate CSV files with the list of public IPs for each AWS region.
Post-Setup Considerations
Permissions: Make sure the AWS IAM user whose credentials you're using has sufficient permissions to list EC2 instances and Elastic IPs across all regions.
Security: Handle your AWS credentials securely. Avoid exposing them in shared or insecure environments.
API Usage and Costs: Be aware of the API call usage, as AWS may charge for excessive API usage depending on your account's billing plan.
By following these steps, you should be able to successfully set up and run the script to list public IPs across all AWS accounts.





