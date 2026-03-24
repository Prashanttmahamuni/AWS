# How to Launch an EC2 Instance in AWS

## Step 1: Name Your Instance
Assign a name to your instance for easy identification. This name is created as a tag where the key is "Name" and the value is the name you provide.

## Step 2: Choose AMI (Operating System)
Select an Amazon Machine Image (AMI). An AMI is a template that contains the operating system and required software to launch the instance.

## Step 3: Choose Instance Type
Select the instance type based on required CPU, memory, storage, and network capacity.

## Step 4: Configure Key Pair
Create or select a key pair for secure login. The public key is stored on the instance and the private key is stored on your local machine.

## Step 5: Configure Network
Launch the instance in a Virtual Private Cloud (VPC) and select a subnet. By default, the instance is launched in a public subnet, which assigns a public IP address and allows internet access.

For testing purposes, default settings can be used. For production environments, assign a public IP only when necessary.

## Step 6: Configure Security Group
A security group acts as a firewall to control traffic.

To allow SSH access:
- Port: 22
- Source: Your IP address (recommended)

For testing, you can allow access from any IP address. For production, restrict access to specific IP addresses.

## Step 7: Configure Storage
Add storage using Amazon EBS. The root volume contains the operating system and required boot files.

## Step 8: Review and Launch
Review all configurations and launch the instance.

## Outcome
The EC2 instance is successfully launched and ready for use.