# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: DIVYA LAKSHMI M
* **Register Number**: 212224040082
* **Date of Submission**: 28-02-2026
---

## Objective

The objective of this experiment is to understand the fundamentals of Amazon Elastic Compute Cloud (EC2). This lab focuses on launching and managing a virtual server, understanding instance types and AMIs, connecting to an EC2 instance, monitoring its status, and performing basic instance operations such as start, stop, and terminate.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity
* Basic knowledge of Linux commands (optional)

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Key Pair
* Security Group
* SSH Client (PuTTY / Terminal)

---

## Tasks Performed

### Task 1: Explore Amazon EC2 Dashboard

Explore the EC2 service dashboard in the AWS Management Console. Observe the different sections such as Instances, AMIs, Instance Types, Key Pairs, Security Groups, and Elastic IPs.

---

### Task 2: Launch an EC2 Instance

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type (t2.micro) under the free tier. Configure basic settings such as instance name, key pair, and security group.

---

### Task 3: Configure Security Group

Configure a security group to allow inbound access:

* SSH (Port 22) from your IP address
* HTTP (Port 80) from anywhere (0.0.0.0/0)

This security group acts as a firewall for the instance.

---

### Task 4: Connect to EC2 Instance

Connect to the running EC2 instance using SSH. Use the downloaded key pair and connect via terminal or PuTTY.

For Amazon Linux:

```
ssh -i "keyname.pem" ec2-user@<Public-IP>
```

---

### Task 5: Perform Basic Instance Operations

Perform the following operations from the EC2 console:

* Stop the instance
* Start the instance
* Reboot the instance

Observe the state changes of the instance.

---

### Task 6: Monitor EC2 Instance

Monitor the EC2 instance using the Monitoring tab. Observe metrics such as CPU utilization, network in/out, and instance status checks.

---

### Task 7: Terminate EC2 Instance

Terminate the EC2 instance after completing the experiment to avoid unnecessary AWS charges.

---

## Workflow (Student Explanation)

1.The EC2 Dashboard was accessed through the AWS Management Console to explore the Amazon EBS volume types.

2.A new EBS volume was created by selecting the volume type, size, and the same Availability Zone as the EC2 instance.

3.The created EBS volume was attached to the running EC2 instance as an additional block device. 

4.The attached volume was formatted using the ext4 file system and mounted to a directory in the EC2 instance. 

5.Sample data was stored in the mounted volume, and after rebooting the instance, data persistence was verified successfully.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List

<img width="1271" height="609" alt="Screenshot 2026-03-08 194006" src="https://github.com/user-attachments/assets/5a373bd1-6cc8-404c-adb4-d49815a4c522" />

<img width="1268" height="608" alt="Screenshot 2026-03-08 193946" src="https://github.com/user-attachments/assets/c430db77-908f-4f4e-b48a-54cfe663b595" />

---

### Screenshot 2: SSH Connection to Instance

<img width="1268" height="797" alt="Screenshot 2026-03-08 193929" src="https://github.com/user-attachments/assets/24193cbe-be67-4be7-b9ff-4b861395de80" />

### Screenshot 3: Instance Monitoring / Status

<img width="1265" height="613" alt="Screenshot 2026-03-08 193913" src="https://github.com/user-attachments/assets/ba213e78-9b15-421a-bfde-99a524a9faf4" />

<img width="1267" height="614" alt="Screenshot 2026-03-08 193850" src="https://github.com/user-attachments/assets/7632b993-887a-4a46-830d-2e7fba41f931" />

---

## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.
