# Week 9: Monitoring and Governance with AWS CloudWatch & CloudTrail

## ✅ Summary
In Week 9, the focus was on configuring and utilizing AWS CloudWatch for resource monitoring and AWS CloudTrail for governance, auditing, and compliance. This week provided hands-on implementation of dashboards, alarm creation, and activity logging across multiple AWS services.

---

## 📂 Directory Structure (Week 9)
```
Week-09-Monitoring-Governance/
├── images/
│   ├── image1.png  # Cloud Foundations Module 10 Knowledge Check Result
│   ├── image2.png  # CloudWatch dashboard with NumberOfObjects and ResourceUsage widgets
│   ├── image3.png  # CloudTrail trail overview for aca-prg-trail-lok
├── README.md
```

---

## 📘 Analysis

### 1. **Cloud Foundations Knowledge Check**  
**<img width="959" alt="image1" src="https://github.com/user-attachments/assets/2c6ede94-5b1e-452c-93c8-69038c902efc" />
**  
- Scored **90%**, indicating strong grasp of AWS Cloud Foundations Module 10.
- Demonstrates clear understanding of monitoring, governance, and account activity tracking.

### 2. **CloudWatch Dashboard Configuration**  
**<img width="959" alt="image2" src="https://github.com/user-attachments/assets/0d2e5409-d4d4-45e7-a464-c2c2b6d7ce67" />
**  
- A CloudWatch Dashboard named **aca-prg-MCR-LOK** was created.
- Two widgets are configured:
  - **NumberOfObjects**: Visualizes object count changes over 3 months.
  - **ResourceUsage**: Shows system resource consumption (very low in this case).
- A CloudWatch **Alarm** named `aca-prg-alarm-lok` is set up to monitor defined thresholds. This is key for real-time alerting and automation.

### 3. **AWS CloudTrail Setup for Auditing**  
**<img width="959" alt="image3" src="https://github.com/user-attachments/assets/bb162b64-08ce-4e38-8a19-918351ecf1e7" />**  
- CloudTrail trail `aca-prg-trail-lok` is created and logging is enabled.
- **Multi-region trail**: Enabled to monitor activity across all regions.
- No SNS notifications or CloudWatch log group integration is enabled yet, which could be added for advanced alerting.
- This allows tracking of all API calls made across AWS, essential for compliance and troubleshooting.

---

## 📌 Key Learnings
- ✅ Configuring custom **CloudWatch Dashboards** and monitoring metrics like S3 object count.
- ✅ Setting up **Alarms** for proactive infrastructure monitoring.
- ✅ Enabling **CloudTrail** for secure auditing and compliance.

---

## 📝 Notes for Screenshots
- **image1.png**: Add this under a folder named `/images` and reference it under the **Knowledge Check** section.
- **image2.png**: Place this under the **CloudWatch Monitoring** subsection.
- **image3.png**: Add to the **CloudTrail Setup** subsection.

---

## 🚀 Next Steps
- Add SNS notifications to CloudTrail for real-time log alerts.
- Integrate CloudWatch alarms with Lambda for automated remediations.
- Use CloudTrail log insights to analyze unusual patterns.

---

## 📁 Commit Message Template
```
feat: Added Week 9 CloudWatch & CloudTrail setup with images and monitoring dashboards
