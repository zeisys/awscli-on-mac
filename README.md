# Install AWS CLI on your Mac Terminal

## Purpose of the Repository

* Check whether AWS Command Line Interface (CLI) is installed on your *Apple Mac / MacBook / MacBook Pro / iMac Terminal*
* Instructions on how to *install AWS CLI*
* Instructions on how to *connect to AWS CLI from your Mac Terminal*
* Spin up your first AWS resource from AWS CLI (*an EC2 instance*)

## Steps to run the Repository

**STEP 1. Open *Terminal* in your Mac**



<p align="center">
  <img src="./Slide1.png" alt="Open terminal in your Mac OS (darwin OS)" width="1300">
</p>



**STEP 2. Ensure you are *super user* who can run *sudo* commands. Execute the following command at the terminal's *prompt*.**

```
sudo -v
```

If you are not a super user, you will get the following error - *Sorry, user <username> may not run sudo on <mac name>.*
  
If you are a super user, you will not get any response.  
  
Please note if you are not a super user, you will **NOT** be able to complete the remaining steps below.


**STEP 3. To find the version of AWS CLI installed, execute at the terminal's *prompt*.**

```
aws --version
```


<p align="center">
  <img src="./Slide2.png" alt="Find version of the AWS CLI installed on your mac" width="1300">
</p>


If AWS CLI is not installed you will get the following error - *No such file or directory*

If AWS CLI is installed, you will get the following message - *aws-cli/X.X.X Python/X.X.X Darwin/X.X.X botocore/X.X.XdevX*


**STEP 4. If AWS CLI is installed, please skip to STEP X**

**STEP 5. If AWS CLI is not installed, you can execute the following command(s) at the prompt:**

Install Homebrew
```
sudo brew install awscli
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
