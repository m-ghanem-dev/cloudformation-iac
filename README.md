# Cloudformation-iac
# Mohamed Ghanem

## Description
The application is a dummy NGINX server deployed in a highly available architecture within a VPC, utilizing two public subnets and two private subnets across separate Availability Zones. Public subnets host the NAT gateways and the load balancer nodes, while private subnets securely run replicas of the service, ensuring fault tolerance, scalability, and network isolation. This design maximizes uptime and protects the application from single points of failure.
The application consists of EC2 instances packed in an autoscaling group which is the target for the load balancer.
The security group of the loadbalancer accepts HTTP connection from any IP address whereas the security group of
the EC2 instances accepts HTTP connections only from the security group of the load balancer


## Spin up instructions
Run the Network CloudFormation Stack workflow.
Choose to the deploy option to spin up or update the resources.

Run the Application CloudFormation Stack workflow.
Choose to the deploy option to spin up or update the resources.

After deployment, obtain the DNS name of the Load Balancer from the stack outputs
and use this URL to access the application (in this example it is a simple NGINX server).

## Tear down instructions

Run the Application CloudFormation Stack workflow.
Choose to the deploy option to spin up or update the resources.

Run the Network CloudFormation Stack workflow.
Choose to the delete option to remove the resources.