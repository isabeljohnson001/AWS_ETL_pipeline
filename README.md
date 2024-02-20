# Automated Data Upload to Amazon S3 from EC2

This repository contains scripts and instructions for automating the upload of CSV files to Amazon S3, utilizing Python and Shell scripting within an AWS EC2 instance environment. The process includes creating a new S3 bucket, fetching a CSV file from a URL, and managing the upload process through automated scripts.

### Tech Stack
Python: For scripting the data retrieval and upload process.
Shell Scripting: To automate the setup and execution of the Python script within EC2.
Amazon S3: As the target storage service for the uploaded CSV files.

### Setup Instructions

- EC2 Instance Setup:
  
Create a new EC2 instance with an attached IAM role (ec2-s3-full-access) allowing S3 access.
Ensure the instance is configured with a Security Group that allows SSH access.

- IAM Role Configuration:

Create an IAM role with AmazonS3FullAccess for the EC2 instance to interact with S3 buckets.

- Python Script Configuration:

Python script (csv_to_s3.py) is used to download a CSV file and upload it to a newly created S3 bucket.

- Shell Script Automation:

Shell script (setup.sh) automates the installation of required packages, execution of the Python script, and management of logs.

- Running the Automation

1.SSH into your EC2 instance.</br>
2.Download setup.sh from the GitHub repository.</br>
3.Execute setup.sh to run the automation process.
