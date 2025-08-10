# Cloudformation-iac
# Mohamed Ghanem

## Description
The application is deployed in a highly available architecture within a VPC, utilizing two public subnets and two private subnets across separate Availability Zones. Public subnets host the NAT gateways, while private subnets securely run replicas of the service, ensuring fault tolerance, scalability, and network isolation. This design maximizes uptime and protects the application from single points of failure.

## Spin up instructions
Run the Network CloudFormation Stack workflow.
Choose to the deploy option to spin up or update the resources.

## Tear down instructions
Run the Network CloudFormation Stack workflow.
Choose to the delete option to remove the resources.