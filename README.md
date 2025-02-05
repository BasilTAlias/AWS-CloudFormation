# Automating Infrastructure Deployment with AWS CloudFormation

## Overview

This project demonstrates the use of AWS CloudFormation to automate the deployment and management of a multi-layer infrastructure. It includes creating a network layer, deploying an application layer, updating infrastructure, and exploring CloudFormation Designer for template visualization.

## Files

1. **`lab-network.yaml`**: Template for deploying the networking layer, including VPC, subnets, and associated resources.
2. **`lab-application.yaml`**: Template for deploying the application layer, including EC2 instances and security groups.
3. **`lab-application2.yaml`**: Updated template for modifying application security settings, such as allowing HTTPS traffic.

# Task 1: Deploying the Network Layer

### Objective
Deploy the foundational networking layer using the `lab-network.yaml` template.

### Steps
1. **Create a CloudFormation Stack**:
   - Use the `lab-network.yaml` template to create a stack named `lab-network`.
   - The stack provisions a VPC, subnets, and other networking components.

2. **Verify Deployment**:
   - Confirm the successful creation of the stack and review the resources created, such as the VPC and subnets.
   - Check the **Outputs** tab in the CloudFormation console for details like VPC ID and subnet IDs.


 $~$
 
  ![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/1.png)

  Current VPC details
  
$~$

  ![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/2.png)

  Creating a new Cloudformation stack by using the template file
  
$~$

  ![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/3.png)

  Stack Creation in Progress

$~$

  ![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/4.png)

  Stack Creation successfully completed

$~$

  ![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/5.png)

  Created resources details

$~$

  ![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/6.png)

  Output tab details

$~$

  ![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/7.png)

  Newly created VPC details

$~$

# Task 2: Deploying the Application Layer

### Objective
Deploy the application layer using the `lab-application.yaml` template, which includes an EC2 instance and a security group.

### Steps
1. **Create a CloudFormation Stack**:
   - Use the `lab-application.yaml` template to create a stack named `lab-application`.
   - Reference the `lab-network` stack to ensure the application layer is deployed within the existing network infrastructure.

2. **Verify Deployment**:
   - Confirm the successful creation of the stack and review the resources created, such as the EC2 instance and security group.
   - Access the web server using the URL provided in the **Outputs** tab.

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/8.png)

Creating a new Cloudformation stack by using the template file

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/9.png)

Stack creationSuccessfully completed 

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/10.png)

Created resources details

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/10-a.png)

EC2 instance detail

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/11.png)

Accessing the web page

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/12.png)

Security group inbound rule details

$~$

# Task 3: Updating the Stack

### Objective
Update the `lab-application` stack to allow HTTPS traffic on port 443 using the `lab-application2.yaml` template.

### Steps
1. **Update the Stack**:
   - Use the `lab-application2.yaml` template to update the `lab-application` stack.
   - Modify the security group to allow HTTPS traffic.

2. **Verify the Update**:
   - Confirm the successful update of the stack.
   - Review the updated security group inbound rules to ensure HTTPS traffic is allowed.

  $~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/13.png)

Updating the stack

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/14.png)

Stack update successfully completed 

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/15.png)

Updated Security Group Inbound Rules

$~$

# Task 4: Exploring AWS CloudFormation Designer

### Objective
Visualize and modify CloudFormation templates using AWS CloudFormation Designer.

### Steps
1. **Visualize Templates**:
   - Open the `lab-network.yaml` and `lab-application2.yaml` templates in AWS CloudFormation Designer.
   - Explore the relationships and interdependencies of resources.

2. **Modify Templates**:
   - Use the drag-and-drop interface to edit or add resources.
   - Experiment with the graphical representation of the infrastructure.

$~$

AWS CloudFormation Designer is a graphical tool for creating, visualizing, and modifying AWS CloudFormation templates. It provides a drag-and-drop interface to diagram resources and their relationships, enabling efficient design and management of infrastructure as code.

$~$

![Alt text of the image](https://github.com/BasilTAlias/AWS-CloudFormation/blob/main/Images/16.png)

Template Visualization in CloudFormation Designer (`lab-application2.yaml` file design)

$~$

# Key Features
- Infrastructure as Code (IaC): Automates resource creation and management.
- Modular Design: Separates networking and application layers for better reusability.
- Template Visualization: Utilizes AWS CloudFormation Designer for enhanced template understanding.
- Update Management: Demonstrates controlled and repeatable stack updates.

$~$
---  

## Conclusion

This project provides a hands-on demonstration of how AWS CloudFormation can be used to automate infrastructure deployment and management. By following the tasks, users can gain a deeper understanding of IaC principles, modular design, and the use of AWS CloudFormation Designer for template visualization and modification.
