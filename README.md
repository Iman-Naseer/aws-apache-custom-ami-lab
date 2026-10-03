# AWS EC2 Apache Deployment & Custom AMI Lab

## Overview
This repository documents a hands-on cloud architecture and server administration lab performed on **Amazon Web Services (AWS)**. The objective of this project was to provision an EC2 instance, install and configure a web server, test custom HTML output, and build a reusable **Amazon Machine Image (AMI)**.

---

## Lab Architecture & Workflow Banner
![EC2 Custom AMI Workflow](ec2-custom-ami-workflow.jfif)

---

## 📂 Lab Documentation
* You can view and download the complete step-by-step lab report with screenshots here: 
  [Download Lab Report PDF](aws-cloud-server-and-ami-walkthrough.pdf)

---

## Step-by-Step Methodology
1. **Instance Creation & Setup**: Provisioned an Amazon Linux 2023 instance (`MYAPACHELAB`) on EC2 using `t3.micro`.
2. **Network & Security Configuration**: Configured security groups to allow inbound SSH and HTTP traffic.
3. **Remote Access & Package Management**: Connected via SSH, updated packages (`yum update`), and installed Apache (`httpd`).
4. **Web Server Customization**: Created a custom HTML landing page displaying `"Hello World FROM CYBERSECURITY ANALYST"`.
5. **Custom AMI Generation**: Created a snapshot image (`APACHELAB`) directly from the running instance.
6. **Deployment & Testing**: Launched a brand-new instance (`AMI-APACHELAB`) from the custom AMI and successfully verified the web output.

---
*By: Iman Naseer*
