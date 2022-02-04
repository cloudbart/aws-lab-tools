# aws-lab-tools
A set of AWS CloudFormation templates for setting up a limited permissions lab user in AWS

# Deployment
- The template will create a limited-permissions lab user restricted to a single AWS Region. 
- Begin by making sure you are in the correct region for your new user. 
- Follow the onscreen options to "Create stack - with new resources"
- In the Amazon S3 URL field, enter in this URL: https://cloudbart-aws-lab-tools.s3.amazonaws.com/BaseParentStack.json
- [Next]
- Answer the prompts on the next page -
  - Stack name: LabToolsStack
  - Limited Permissions Lab User: username for the new lab user
  - Where to send the alerts?: valid email address to have billing alerts sent to
- [Next]
- Make sure to scroll down and check the two permissions options for allowing CloudFormation to create IAM resources and to run nested templates
- [Create stack]

Log in using the new labuser you defined, the default password is LabPass1 and you'll be prompted to change it at first login. Make sure it fits the AWS complexity requirements.

