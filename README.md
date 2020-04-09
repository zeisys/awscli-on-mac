# Purpose of the Repository

* To deploy containerized pipeline tools Jenkins, SonarQube, and Selenium, to an AWS ECS EC2 Cluster.
* To trigger the continuous integration of a hello world Java application from an external GitHub repo's pac
* Note: Continuous deployment of the hello world Java application will ***NOT*** happen



How to install AWS Command Line Interface (CLI) on your Mac / MacBook / iMac terminal. 

**1. To find the version of AWS CLI installed, execute at the prompt:**
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
