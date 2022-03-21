# multicloud

#### deploys a simple two layer network including needed gateways to AWS via different approaches:

0. via AWS CloudFormation
1. via Terraform through AWS CLI 
2. via Terraform through Terraform Cloud

#### this example describe the migration path to be able to deploy infrastructure via terraform to multiple cloud platforms:

0. AS-IS: infrastructure as code is available in AWS CloudFormation
1. Migrating the AWS CloudFormation code to Terraform:
   1. enabling own state handling
   2. enabling module structure
   3. enabling dynamic infrastructure by usage of "count" feature
2. Usage of Terraform Cloud as central deployment platform
   1. enabling central state handling
   2. enabling collaboration
   3. enabling overview for multi cloud deployments
3. TO-BE: add terraform infrastructure-as-code for more cloud provider
   1. add network module for next cloud provider with stable interface
   2. use stable network configuration to different cloud provider

# two layer network
![network module](doc/network.png "network module")