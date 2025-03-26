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

![image1](https://github.com/user-attachments/assets/11ae3f0f-f24a-4f07-b50b-bb1e46b24ac8)
![image2](https://github.com/user-attachments/assets/ab28df01-d9a1-4833-8785-5151e0483958)
![image3](https://github.com/user-attachments/assets/c389a677-1d89-4d09-ab29-1296396c6236)
![image4](https://github.com/user-attachments/assets/08a7423f-ca57-48ef-8ca8-2a343b8571ec)
![image6](https://github.com/user-attachments/assets/849f6ed2-ce8d-4e44-a794-d9ecfae8fd95)
![image5](https://github.com/user-attachments/assets/74d1b350-0a0f-44f4-9fa6-04a7418cb4e2)
![image9](https://github.com/user-attachments/assets/8cdf14c8-a203-477e-b0d8-bd1ff655a1c5)
![image7](https://github.com/user-attachments/assets/3d9dd948-7c3e-4644-a57f-88e1277dc2dc)
![image8](https://github.com/user-attachments/assets/50848cfe-a9d9-41f0-81c2-a43d2be87389)
