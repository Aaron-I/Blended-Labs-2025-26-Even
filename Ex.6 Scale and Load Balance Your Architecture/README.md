# Lab 6 – Scale and Load Balance Your Architecture

## Title

Scale and Load Balance Your Architecture

**Author : Aaron I**
**Reg no : 212223230002**   
**Date : 22/05/2026**

---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow (To be filled by Student)
1. Logged in to the AWS Management Console and reviewed the existing EC2 infrastructure, VPC, and security groups created in previous labs.
2. Created a Launch Template by selecting the required AMI, instance type, security group, and user data script.
3. Created an Auto Scaling Group (ASG) using the launch template and configured the desired, minimum, and maximum instance capacities.
4. Configured the Application Load Balancer (ALB) and attached the Auto Scaling Group to the existing target group (LabGroup) for traffic distribution.
5. Configured Auto Scaling policies based on CPU utilization and enabled CloudWatch monitoring to automatically scale instances according to workload.
6. Tested the architecture by generating traffic, verified load balancing across EC2 instances, and observed automatic scaling actions through CloudWatch and Auto Scaling activities.

---

## Output Screenshots 

Load Balancer

<img width="1917" height="965" alt="image" src="https://github.com/user-attachments/assets/134c71e6-c560-4790-8bc2-e6f4fa35cc0f" />

Auto Scaling Group 

<img width="1919" height="965" alt="Screenshot 2026-05-30 115241" src="https://github.com/user-attachments/assets/3d7a4ebc-d6dd-4ce7-a9d0-0e2c0047da51" />

CloudWatch Alarms Created

<img width="1915" height="965" alt="image" src="https://github.com/user-attachments/assets/ba956e04-4fa0-4760-b327-1137511e0ee6" />

---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
