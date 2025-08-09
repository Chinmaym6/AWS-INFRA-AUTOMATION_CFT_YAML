# CloudWatch Alarm for EC2 CPU Utilization with SNS Email Notifications

This project creates a **CloudWatch Alarm** to monitor CPU utilization of a specific EC2 instance.  
When the CPU usage exceeds a defined threshold, an **SNS notification** is sent to a specified email address.

---

## 🏗️ Code Steps

1. **Create an SNS Topic** (Simple Notification Service).
2. **Create an SNS Subscription** with your email address.
3. **Create a CloudWatch Alarm** (e.g., CPUUtilization ≥ 80%).
4. **Link the CloudWatch Alarm** to the SNS Topic for alert notifications.

---

## 🚀 Deployment Steps

1. Go to **AWS Management Console**.
2. Navigate to **CloudFormation**.
3. Click **Create Stack** → **With new resources (standard)**.
4. Choose **Upload a template file**, **Specify an Amazon S3 template URL**, or **Sync to GitHub**.
5. Upload your **YAML** file and click **Next**.
6. Enter the stack name and parameters.
7. Review the settings and click **Create stack**.
8. Wait for the stack creation to complete.
9. Once created, check the **CloudFormation** console for resources.
10. You will receive an **email** to confirm subscription to the SNS topic.
11. After confirming, you will get email alerts when CPU utilization exceeds the set limit.
12. You can also check the **CloudWatch** console for the created alarm and its status.

---

## 📌 Notes
- Ensure your EC2 instance is running and **CloudWatch metrics** are enabled.
- The email subscription must be **confirmed** before receiving alerts.
