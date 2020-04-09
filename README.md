# Install AWS CLI on your Mac Terminal

## Purpose of the Repository

* Check whether AWS Command Line Interface (CLI) is installed on your *Apple Mac / MacBook / MacBook Pro / iMac Terminal*
* Instructions on how to *install AWS CLI*
* Instructions on how to *connect to AWS CLI from your Mac Terminal*
* Spin up your first AWS resource from AWS CLI (*an EC2 instance*)


**STEP 1. Open the Terminal in your Mac**




**STEP 1. To find the version of AWS CLI installed, execute at the prompt:**
```
aws --version
```

**8. If AWS CLI is not installed, then on a Mac Terminal, you can execute the following command(s) at the prompt:**

Install Homebrew
```
brew install awscli
```

Configure AWS CLI credentials 
```
aws configure
```

Check your connectivity to AWS
```
aws sts get-caller-identity
```
*If the connectivity is established, you will get your UserID, AWS Account Number, and your IAM ARN in AWS. *

**9. In your mac terminal, git clone this repository**
