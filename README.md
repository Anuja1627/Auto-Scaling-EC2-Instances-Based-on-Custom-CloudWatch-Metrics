# 🔄 Auto Scaling EC2 Instances Based on Logged-In Users

This project demonstrates how to automatically scale AWS EC2 instances based on the number of users logged into a custom web application using:

- 🟢 **CloudWatch** for custom metrics
- 🧩 **Auto Scaling Groups (ASG)** for EC2 scaling
- ⚙️ **Launch Templates** for instance configuration
- 🐚 Bash scripts to push custom metrics

---

## 📌 Overview

The use case: As user load increases on a custom application, automatically add EC2 instances. As the load decreases, remove them. This scaling is based on a custom CloudWatch metric representing the number of active users.

---

🔐 AWS Setup
An AWS account with necessary IAM permissions to:

Launch EC2 instances

Create Auto Scaling Groups

Create Launch Templates

Create and publish custom CloudWatch metrics

Default VPC and Subnets configured (or create custom ones)

Key Pair for SSH access to EC2 instances

