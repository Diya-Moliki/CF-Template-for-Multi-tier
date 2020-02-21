# Cloudformation


STEP 1: Install AWS CLI on a linux machine by running the command below
===================================================================
curl "https://s3.amazonaws.com/aws-cli/awscli-bundle.zip" -o "awscli-bundle.zip"

unzip awscli-bundle.zip

sudo ./awscli-bundle/install -i /usr/local/aws -b /usr/local/bin/aws



STEP 2: Add your Access Key ID and Secret Access Key to ~/.aws/config using this format:
===============================================================================
[default]

aws_access_key_id = <access key id>
  
aws_secret_access_key = <secret access key>
  
region = us-west-2




STEP 3: Protect the config file:
=======================
chmod 600 ~/.aws/config



STEP 4: Clone the cloud formation script by running the following command
=========================================================================
cd /

git clone  https://github.com/Kwara1989/Cloudformation.git

cd Cloudformation



STEP 5: To launch  stack. RUN THE cf_auto.template SCRIPT LIKE THIS
=====================
aws cloudformation create-stack --region us-west-2b --stack-name autoPeople --template-body

file:///Cloudformation/cf_auto.template 



