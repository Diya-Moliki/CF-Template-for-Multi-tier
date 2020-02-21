# Cloudformation


STEP 1: Install AWS CLI on a linux machine by running the command below
===================================================================
curl "https://s3.amazonaws.com/aws-cli/awscli-bundle.zip" -o "awscli-bundle.zip"

unzip awscli-bundle.zip

sudo ./awscli-bundle/install -i /usr/local/aws -b /usr/local/bin/aws



STEP 2: configure aws cli by running "aws configure" command
===============================================================================

aws_access_key_id = <access key id>
  
aws_secret_access_key = <secret access key>
  
region = us-west-2

output = json




STEP 3: Clone the cloud formation script by running the following command
=========================================================================
cd /

sudo git clone  https://github.com/Kwara1989/Cloudformation.git

cd Cloudformation



STEP 4: To launch  stack. RUN THE cf_auto.template SCRIPT LIKE THIS
=====================
aws cloudformation create-stack --region us-west-2 --stack-name autoPeople --template-body file:///Cloudformation/cf_auto.template 


STEP 5: To ssh into the provisioned server
=====================
Note: wait for the server to be fully provisioned on AWS then,

ssh sysadmin@ipaddress

start nginx server if not running or check status 

copy and paste your public ipaddress to the browser. 



