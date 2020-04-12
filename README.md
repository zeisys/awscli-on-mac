# Install AWS CLI on your Mac Terminal

## Purpose of the Repository

* Check whether AWS Command Line Interface (CLI) is installed on your *Apple Mac / MacBook / MacBook Pro / iMac Terminal*
* Instructions on how to *install AWS CLI*
* Instructions on how to *connect to AWS CLI from your Mac Terminal*
* Spin up your first AWS resource from AWS CLI (*an EC2 instance*)

## Steps to run the Repository
<br/>

**STEP 1. Open *Terminal* in your Mac**

<br/>

<p align="center">
  <img src="./Slide1.png" alt="Open terminal in your Mac OS (darwin OS)" width="1300">
</p>

<br/>

**STEP 2. Ensure you are *super user* who can run *sudo* commands. Execute the following command at the terminal's *prompt*.**

```
sudo -v
```

If you are not a super user, you will get the following error - *Sorry, user <username> may not run sudo on <mac name>.*
  
If you are a super user, you will not get any response.  
  
Please note if you are not a super user, you will **NOT** be able to complete the remaining steps below.

<br/>

**STEP 3. To find the version of AWS CLI installed, execute at the terminal's *prompt*.**

```
aws --version
```

<br/>

<p align="center">
  <img src="./Slide2.png" alt="Find version of the AWS CLI installed on your mac" width="1300">
</p>


If AWS CLI is not installed you will get the following error - *No such file or directory*

If AWS CLI is installed, you will get the following message - *aws-cli/X.X.X Python/X.X.X Darwin/X.X.X botocore/X.X.XdevX*

<br/>


**STEP 4. If AWS CLI is installed, please skip to STEP X**

<br/>

**STEP 5. If AWS CLI is not installed, the first step is to install *Homebrew*.**

Homebrew is a package manager for macOS. Please refer https://brew.sh/ for more information. To install Homebrew please paste the following command at the prompt.

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

<br/>

**STEP 5. Now you can install the *AWS CLI package*.**

Paste following command at the prompt
```
brew install awscli
```

If you get a message saying *Error: The following directories are not writable by your user:*, you must prefix *sudo* with each of your commands at the prompt as shown below.
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
