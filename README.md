# Infrastructure

1. Clone the repository to get the CloudFormation Template ```csye6225-infra.yml```
2. Run the following command in AWS CLI:

```bash
aws cloudformation deploy --profile demo --template-file csye6225-infra.yml --region us-east-1 --capabilities CAPABILITY_NAMED_IAM --parameter-overrides KeyName=testkey AMIImage=ami-0174c366a73162742 --stack-name test
```
3. To cleanup the stack, use the following command in the AWS CLI:

```bash
aws cloudformation delete-stack --stack-name <insert_stack_name> --profile <insert_profile> --region <insert_region>
```
