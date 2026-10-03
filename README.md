# AWS EC2 Apache Deployment & Custom AMI Lab

## Overview
This repository documents a hands-on cloud architecture and server administration lab performed on **Amazon Web Services (AWS)**. The objective of this project was to provision an EC2 instance, install and configure a web server, test custom HTML output, and build a reusable **Amazon Machine Image (AMI)**.

---

## Lab Architecture & Workflow

### 1. Instance Creation & Configuration
* **Service:** Amazon EC2
* **Instance Name:** `APACHELAB` / `AMI-APACHELAB`[cite: 1]
* **Software Image (AMI):** Amazon Linux 2023 (x86_64)[cite: 1]
* **Instance Type:** `t3.micro` (Free Tier eligible)[cite: 1]
* **Network Settings:** Configured security groups to allow inbound **SSH (Port 22)** and **HTTP (Port 80)** traffic from anywhere (`0.0.0.0/0`)[cite: 1].

### 2. Remote Access & Web Server Installation
* Connected to the instance remotely via SSH using terminal tools[cite: 1].
* Updated system package repositories using `sudo yum update -y`[cite: 1].
* Installed the **Apache HTTP Server** using `sudo yum install -y httpd`[cite: 1].
* Started and enabled the Apache service using:
  ```bash
  sudo systemctl start httpd.service
  sudo systemctl enable httpd.service
