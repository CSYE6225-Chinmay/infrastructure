# CloudFormation Template to create VPC's

1. Clone the repository using git clone
2. Open AWS CLI at the folder

3. Run the following command with desired parameters to create stack:
> `aws cloudformation create-stack --template-body file://csye6225-infra.json --stack-name test1 --profile dev --region us-east-1 --parameters ParameterKey=EnvironmentName,ParameterValue=dev ParameterKey=VpcCIDR,ParameterValue=10.0.0.0/16 ParameterKey=PublicSubnet1CIDR,ParameterValue=10.0.1.0/24 ParameterKey=PublicSubnet2CIDR,ParameterValue=10.0.2.0/24 ParameterKey=PublicSubnet3CIDR,ParameterValue=10.0.3.0/24`

4. You can check the status of your stack in your dev aws account

5. To cleanup the stack run the following command:
> `aws cloudformation delete-stack --stack-name test3 --profile dev --region us-east-2`
