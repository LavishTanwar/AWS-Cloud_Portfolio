# Week 5 - AWS Cloud Portfolio Implementation

## ✅ Overview

In Week 5, the focus was on **data enrichment** and **cost-efficient summarization** using AWS Glue and S3. This week's work expanded on earlier data preparation workflows by introducing **joins** between datasets and optimizing Glue job configurations for performance and cost analysis.

---

## 📌 Objectives

- Enrich faculty and preliminary data using AWS Glue.
- Create consolidated datasets and output to multiple S3 targets.
- Analyze cost and performance of Glue job execution.
- Validate output schema in Glue Data Catalog.

---

## ⚙️ Key Tasks & Activities

### 1. **Glue Job Creation: Faculty-Preliminary**
- Joined **Faculty** and **Preliminary** datasets using a **Join transform**.
- Combined data written to:
  - `/system/` directory on S3
  - `/User/` directory on S3
- Converted to single output file before writing to targets.

📸 *Visual Reference*:  
![image1](https://github.com/user-attachments/assets/f85ea89a-e969-4bc1-8b6f-d0290b482824)

- Screenshot: `Faculty-Preliminary` Glue Visual ETL  
- S3 Outputs:
  - `academics-cur-lok/Faculty-Preliminary/system/`
  - `academics-cur-lok/Faculty-Preliminary/User/`

---

### 2. **Data Summarization Cost Analysis**
- Tracked:
  - Number of Glue sessions
  - Job nodes used
  - Glue job duration per execution
- Created summary table:
Glue Iteration	Sessions	Nodes	Duration
Iteration 1	2	10	2.25 mins
Iteration 2	2	10	1.50 mins
Iteration 3	2	10	1.57 mins

📸 *Visual Reference*: Data Cost Summary Table in diagrams.net

---
![image2](https://github.com/user-attachments/assets/d081a7a4-9515-494e-97bf-30adcba903e4)

### 3. **Schema Validatio![Uploading image2.png…]()
n**
- Verified schema under table: `faculty performance metrics`
- Located in Glue Data Catalog.
- Data stored in S3 path:  
  `s3://academics-cur-lok/faculty-performance/metrics/System/`
- Columns:
  - `department` (string)
  - `avg_teachingscore_#0` (double)
  - `report_date_ltz` (timestamp)

📸 *Visual Reference*: Final schema verification screenshot.

---
![image3](https://github.com/user-attachments/assets/d02892d6-36ba-4688-ad9f-8736cf1b7abd)

## 📂 Outputs Generated

| Resource                    | Description                               |
|-----------------------------|-------------------------------------------|
| Glue Job                    | `Faculty-Preliminary`                     |
| S3 Output Path (System)     | `s3://academics-cur-lok/Faculty-Preliminary/system/` |
| S3 Output Path (User)       | `s3://academics-cur-lok/Faculty-Preliminary/User/`   |
| Glue Catalog Table          | `faculty performance metrics`             |
| Format                      | Parquet                                   |

---



## 📈 Learnings!
[image4](https://github.com/user-attachments/assets/88a5880a-f46d-4d16-b6e8-b4c8c9dcbe61)
![image5](https://github.com/user-attachments/assets/5887278b-48ff-4ef0-81fe-3e881479dbb2)


- Effective Glue job design for **joining datasets**.
- Managing **output to multiple S3 locations**.
- Interpreting and optimizing **cost metrics** of AWS Glue ETL jobs.
- Understanding schema inheritance and validation through the AWS Glue Data Catalog.

---

✅ **Completed all Week 5 tasks successfully.**

Name - Lokesh Kumar
