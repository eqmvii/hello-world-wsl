# AWS Notes

Setting things up

## CLI Install

aws --version
Command 'aws' not found, but can be installed with:

using snap package since WSL has that:

sudo snap install aws-cli --classic

aws --version
aws-cli/2.22.18 Python/3.12.6 Linux/5.15.167.4-microsoft-standard-WSL2 exe/x86_64.ubuntu.24

:toot: 

## User via IAM user

IAM Identity Center enabled for a non-organization, created a non-root account for myself

That went crazy since I didn't select an organization. Doing it the old and less recommended way (IAM users) for now, will try identity center for next project?

added to admin group

went to user > security credentials to create an access key

## aws configure

$ aws configure
AWS Access Key ID [None]: $KEY
AWS Secret Access Key [None]: $SECRET_KEY
Default region name [None]: us-east-1
Default output format [None]: json

Create or open the shared AWS credentials file. This file is ~/.aws/credentials

## Permissions

Created group and adder user to it 

## Do a thing

wadmin@eqmvii-legionP5:~/repos/hello-world-wsl$ aws s3 ls
2022-02-18 19:47:01 [BUCKET NAME 1]
2018-06-24 14:17:27 [BUCKET NAME 2]

IT WORKED