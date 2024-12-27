# Automating Infrastructure Deployment with AWS CloudFormation

## Overview

This project demonstrates the use of AWS CloudFormation to automate the deployment and management of a multi-layer infrastructure. It includes creating a network layer, deploying an application layer, updating infrastructure, and exploring CloudFormation Designer for template visualization.

## Files

- lab-network.yaml: Template for deploying the networking layer.
- lab-application.yaml: Template for deploying the application layer.
- lab-application2.yaml: Updated template for modifying application security settings.

# Task 1: Deploying the Network Layer

1. Template: lab-network.yaml.
2. Steps:
   - Create a CloudFormation stack named lab-network.

  ![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/1.png)

  VPC details
  
$~$

  ![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/2.png)

  Creating new Cloudformation stack by using template file
  
$~$

  ![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/3.png)

  creation in progress

$~$

  ![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/4.png)

  successfully completed

$~$

  ![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/5.png)

  created resources details

$~$

  ![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/6.png)

  Output tab details

$~$

  ![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/7.png)

  newly created VPC details

$~$

# Task 2: Deploying the Application Layer

1. Template: lab-application.yaml
2. Steps:
   - Create a stack named lab-application referencing lab-network.
   - Deploy an EC2 instance with a security group.
   - Verify the web server by accessing the output URL.

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/8.png)

Creating new Cloudformation stack by using template file

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/9.png)

Successfully completed stack creation

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/10.png)

created resources details

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/10-a.png)

EC2 instance detail

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/11.png)

Accessing web page details

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/12.png)

Security group inbound rule details

$~$

# Task 3: Updating the Stack

1. Template: lab-application2.yaml.
2. Steps:
- Update the lab-application stack to allow HTTPS traffic on port 443.
- Verify the security group’s inbound rules for the new configuration.

  $~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/13.png)

Updating stack

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/14.png)

Successfully updated 

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/15.png)

Security group inbound rule details

$~$

# Task 4: Exploring AWS CloudFormation Designer

1. Tools: AWS CloudFormation Designer.
2. Steps:
- Visualize and modify templates (lab-network.yaml and lab-application2.yaml).
- Explore relationships and interdependencies of resources.
- Experiment with drag-and-drop features to edit or add resources.

$~$

AWS CloudFormation Designer is a graphical tool for creating, visualizing, and modifying AWS CloudFormation templates. It provides a drag-and-drop interface to diagram resources and their relationships, enabling efficient design and management of infrastructure as code.

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/16.png)

lab-application2 yaml file design details

$~$

# Key Features
- Infrastructure as Code (IaC): Automates resource creation and management.
- Modular Design: Separates networking and application layers for better reusability.
- Template Visualization: Utilizes AWS CloudFormation Designer for enhanced template understanding.
- Update Management: Demonstrates controlled and repeatable stack updates.

  
