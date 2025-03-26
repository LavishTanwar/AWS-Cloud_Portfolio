# 📅 Week 2: AWS Cloud Services Basics – EC2, S3 & CloudWatch

## ✅ Objective
This week's tasks focused on deploying basic AWS infrastructure and understanding core services like EC2, S3, and CloudWatch. It included launching an EC2 instance, configuring billing alerts, uploading to S3 via PowerShell, and identifying IAM/connection issues.

---

## 🛠️ Services Used
- **Amazon EC2:** Instance creation & access
- **Amazon S3:** Bucket creation & file upload (via PowerShell)
- **Amazon CloudWatch:** Billing alerts
- **IAM Roles & Permissions**
- **Remote Desktop & PowerShell**

---

## 🔍 Activities Performed

### 1. ✅ Created a Billing Alarm in CloudWatch  
Alarm was set to trigger if estimated charges exceed $10.

---

### 2. ✅ Created S3 Bucket `academics-raw-lok`  
Region: US East (N. Virginia)

---

### 3. ✅ Created folders inside the S3 Bucket  
Folders: `faculty-performance/`, `panel-members/`, `preliminary-feedback/`

---

### 4. ✅ Launched EC2 Windows Instance (t3.micro)  
Instance ID: i-0e95d50239efafa0d

---

### 5. ✅ Logged into EC2 via RDP  
EC2 instance desktop accessed using Remote Desktop.

---

### 6. ✅ Uploaded File from EC2 using PowerShell  
```powershell
write-s3object -bucket academics-raw-lok -file "C:\Users\Administrator\Documents\Panel-members.csv" `
-key "academics/panel-members/year-2025/quarter-1/server-AGVS-LOK/Panel-members.csv"
![image9](https://github.com/user-attachments/assets/d100e584-ceb2-4719-8504-3583828091a7)
![image8](https://github.com/user-attachments/assets/fa8f519f-cff9-4f94-8431-8e97c3d9d5fe)
![image7](https://github.com/user-attachments/assets/66e3518a-12da-4b68-ab94-b50c2a0b7dc0)
![image6](https://github.com/user-attachments/assets/9164c66f-b30b-451c-bf7c-79691f0251f1)
![image5](https://github.com/user-attachments/assets/404ba8d8-bb74-4cd5-b28d-0c5f93bef9be)
![image4](https://github.com/user-attachments/assets/9a071af6-de0d-41c2-a780-f7d1a0df73cf)
![image3](https://github.com/user-attachments/assets/99be0b06-766a-4070-97ef-f7de0a38688a)
![image2](https://github.com/user-attachments/assets/e80aff56-c21a-4bde-b7ac-6c0e3b6e8783)
![image1](https://github.com/user-attachments/assets/0a7b50a5-6885-4806-8840-f9d6a77de4b7)

