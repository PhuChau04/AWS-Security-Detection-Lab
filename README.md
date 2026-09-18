<h1>From Network to Cloud: AWS Security Detection Lab</h1>
 
 [View the Full Lab Walkthrough](LAB-Walkthrough/LAB-WALKTHROUGH.md)

<h2>Description</h2>
Built a simulated AWS environment using LocalStack and Docker to demonstrate cloud security concepts through hands-on testing. The project explores S3 and IAM misconfigurations, remote exploitation from Kali Linux, and the development of a Python/Boto3 detection script to identify publicly exposed S3 buckets.
<br />

<h2>Languages and Utilities Used</h2>

- <b>Python</b>
- <b>Boto3</b>
- <b>AWS CLI</b>
- <b>Docker</b>
- <b>LocalStack</b>

<h2>Environments Used</h2>

- <b>Ubuntu Server</b>
- <b>Kali Linux</b>
- <b>VMware Workstation</b>

<h2>Key Skills Demonstrated</h2>

- <b>AWS CLI</b>
- <b>S3 Security</b>
- <b>IAM Permissions</b>
- <b>LocalStack</b>
- <b>Docker</b>
- <b>Boto3</b>
- <b>Python Scripting</b>
- <b>Cloud Misconfiguration Testing</b>
- <b>Security Detection</b>

<h2>Key Takeaways</h2>

- <b>Gained hands-on experience configuring and managing simulated AWS services using LocalStack and AWS CLI.</b>
- <b>Demonstrated how S3 and IAM misconfigurations can expose data and provide users with excessive permissions.</b>
- <b>Used Kali Linux to test and validate cloud security weaknesses from a remote system.</b>
- <b>Developed a Python/Boto3 detection script to identify publicly accessible S3 buckets.</b>
- <b>Practiced the full security workflow of building, misconfiguring, exploiting, detecting, and validating a cloud environment.</b>

<h2>Milestone 1 - Building the Simulated AWS Environment</h2>
The first milestone focused on creating a simulated AWS environment using LocalStack running inside Docker on an Ubuntu VM. LocalStack provided locally hosted AWS services that could be accessed using the standard AWS CLI through port 4566.

After verifying that the LocalStack container was running successfully, I configured the AWS CLI to communicate with the local environment. I then tested S3 functionality by creating a bucket, uploading and downloading a test file, and verifying its contents.

Finally, I created an IAM user and attached a ReadOnlyAccess policy to verify IAM functionality. This established the working cloud environment that would later be intentionally misconfigured and tested from Kali Linux.

<h2>Milestone 2 — Exploiting and Detecting S3 & IAM Misconfigurations</h2>
The second milestone focused on intentionally introducing security weaknesses into the simulated AWS environment and testing whether they could be exploited and detected. I configured an exposed S3 bucket and an over-permissioned IAM user, tested the weaknesses remotely from Kali Linux, and developed a Python detection script to identify publicly accessible S3 buckets.

