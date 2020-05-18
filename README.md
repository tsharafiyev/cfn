Download the files and run

## This Command to check
aws cloudformation validate-template \
--template-body file://ec2.yaml

## This Command to create a stack

aws cloudformation create-stack \
--stack-name vpc-cli \
--template-body file://vpcOhio.yaml

## This Command Updates a stack
aws cloudformation update-stack \
--stack-name vpc-cli \
--template-body file://vpcOhio.yaml

## Create ec2 command

aws cloudformation create-stack \
--stack-name ec2-stack2 \
--template-body file://ec2.yaml

## Run command with params

aws cloudformation create-stack --stack-name public-ec2 \
--template-body file://ec2.yaml \
--parameters Parameters

aws cloudformation create-stack --stack-name
public-ec2-cli \
    --template-body file://ec2.yaml \
    --parameters file://params.json