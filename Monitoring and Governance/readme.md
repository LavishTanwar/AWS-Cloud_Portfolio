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
**![image1](https://github.com/user-attachments/assets/7787a52e-8ad9-4481-ac40-1e82c1afc39f)

**  
- Scored **90%**, indicating strong grasp of AWS Cloud Foundations Module 10.
- Demonstrates clear understanding of monitoring, governance, and account activity tracking.

### 2. **CloudWatch Dashboard Configuration**  
**![image2](https://github.com/user-attachments/assets/b30773dc-2a2f-481b-8bec-bc09cf6e2192)

**  
- A CloudWatch Dashboard named **aca-prg-MCR-LOK** was created.
- Two widgets are configured:
  - **NumberOfObjects**: Visualizes object count changes over 3 months.
  - **ResourceUsage**: Shows system resource consumption (very low in this case).
- A CloudWatch **Alarm** named `aca-prg-alarm-lok` is set up to monitor defined thresholds. This is key for real-time alerting and automation.

### 3. **AWS CloudTrail Setup for Auditing**  
**![image3](https://github.com/user-attachments/assets/66fc793d-7424-4781-9258-d6e5fe6d7e8c)
**  
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
