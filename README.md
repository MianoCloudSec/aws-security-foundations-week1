# AWS Security Foundations – Week 1

AWS Security Foundations project – Week 1 tasks including MFA, IAM roles, budgets, and alarms.

## Overview
The goal was to set up secure access to AWS resources using the **AWS Well-Architected Framework** and the **Shared Responsibility Model**.

## Steps Completed

### 1. Root Account Security
- Turned on **Multi-Factor Authentication (MFA)** for the AWS root account.
- This helps stop unauthorized access to the most important account.

**Screenshot:**  
![MFA Enabled](https://github.com/MianoCloudSec/aws-security-foundations-week1/blob/main/screenshots/proof%20of%20mfa.png)

---

### 2. IAM User & Groups Setup
- Created an **Admin group** with full permissions.
- Made a separate **Admin IAM user** and added it to the Admin group.
- Created a **ReadOnly IAM user** for testing.
- Checked least privilege by trying to make an S3 bucket with ReadOnly user (failed as expected).

**Screenshot:**  
![ReadOnly Test](https://github.com/MianoCloudSec/aws-security-foundations-week1/blob/main/screenshots/readonly%20proof.png)

---

### 3. AWS Budget Setup
- Created an AWS monthly budget to monitor spending.

**Screenshot:**  
![Budget](https://github.com/MianoCloudSec/aws-security-foundations-week1/blob/main/screenshots/budget%20proof.png)

---

### 4. AWS Budget Alarm Setup
- Added a budget alarm to get alerts if spending gets close to the limit.

**Screenshot:**  
![Budget Alarm](https://github.com/MianoCloudSec/aws-security-foundations-week1/blob/main/screenshots/budgetalarm.png)
