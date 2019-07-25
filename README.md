# multinode-hdp-cluster

One Click Automation of creation and deployment of multi-node HDP cluster using Iac on AWS.

## Getting Started

These instructions will help you setup 'One Click Automation' of manual creation and deployment of a multi-node HDP cluster on Amazon Web Services.

### Prerequisites

1.AWS Account
  1.a Knowledge of EC2 (Elastic Cloud Compute)
  1.b Knowledge of CFT (Cloud Formation Template)
  1.c Knowlege of S3 (Simple Storage Service)
2.Knowledge of Shell Script
3.Knowledge of Python

```
->Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers. 
->AWS CloudFormation simplifies provisioning and management on AWS. You can create templates for the service or application architectures you want and have AWS CloudFormation use those templates for quick and reliable provisioning of the services or applications (called “stacks”). You can also easily update or replicate the stacks as needed.
->Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. 
```

### Preparing for One Click Automation:

1:Log into you AWS Account.
2:Goto s3 service.
3:Create a bucket.
4.Upload the Python folder which contains the python Script to retrive Private-Dns of required EC2 instances and map those into ambari blueprint mapping file.
4:Upload the blue print folder which has the Ambari Blueprint and Mapping file.
5.Open The Coud Formation json file and and go to for each instance user data,here edit the aws cli command according to your s3 bucket.
6.Save changes.


## Execution

1.Upload The Cloud Formation Template file in AWS CFT.
2.Select the required instances type.
3.Select required number of instances (nodes).
3.Select your key.
4.Check the prompt regarding IAM roles.
5.Click on Create Stack

### Output

1.Click on the URL displayed in output section of CFT after your stack is created
2.Log in into Amabari
3.Here you can see all the services installing
4.The installation will finish in 20-30 minutes


### You have succesfully automated the creation and deployment of multi-node HDP cluster.

Next time onwards you only need to upload the json file and create a stack to create and deploy a HDP multi-n0de cluster


## Built With

* [AMAZON WEB SERVICES](https://docs.aws.amazon.com/) - Cloud service used
* [SHELL SCRIPT](https://www.gnu.org/software/bash/manual/html_node/Shell-Scripts.html) - Scripting language
* [PYTHON](https://docs.python.org/3/) - Programming language


## Authors

* **Amar Walke** - *Initial work* - [amarwalke95](https://github.com/amarwalke95)


## Acknowledgments

* Guided By : Pradeep Tripathi - [amarwalke95](https://github.com/amarwalke95)

