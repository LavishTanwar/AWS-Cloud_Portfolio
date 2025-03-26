# Week 5 Cloud Portfolio - README.md

## ✅ Overview
In Week 5, the focus was on **joining datasets**, **data enrichment**, and **job optimization** using AWS Glue Studio. We built and executed the `Faculty-Preliminary` join job, monitored its output in S3, and validated data transformation and storage. 

---

## 📁 Project Structure
```
aws-cloud-portfolio/
├── week5/
│   ├── glue-jobs/![image5](https://github.com/user-attachments/assets/d140033e-562c-40a5-bd7f-20490263a2a8)
![image4](https://github.com/user-attachments/assets/457451e3-dc24-481e-967a-441e2401b910)
![image3](https://github.com/user-attachments/assets/7ed3c552-1ad8-4111-a7aa-3ec143380edf)
![image2](https://github.com/user-attachments/assets/76c9d02c-51ad-4e65-ad1d-2e338c97dcd8)
![image1](https://github.com/user-attachments/assets/2fb9b3de-36f2-4c14-ac40-b65aba70a223)

│   │   └── Faculty-Preliminary
│   ├── s3-outputs/
│   │   ├── system/               --> parquet output of joined data
│   │   └── user/                 --> CSV formatted data
│   ├── diagrams/
│   │   └── architecture.png     --> updated architectural diagram
│   └── analytics/
│       └── cost-analysis.png    --> summarization cost metrics
```

---

## 🔨 Activities Completed

### 1. **AWS Glue Studio: Join Job**
- **Job Name:** `Faculty-Preliminary`
- **Steps:**
  - Extracted data from **Faculty** and **Preliminary Feedback** datasets.
  - Applied **Join transform** (Left Join).
  - Converted joined output into a single file.
  - Output written to two targets:
    - **Parquet** format in `system/`
    - **CSV** format in `user/`

### 2. **S3 Output Verification**
- **System folder:** `Faculty-Preliminary/system/`
  - File: `parquet.snappy`, size: 1010 B
- **User folder:** `Faculty-Preliminary/User/`
  - File: `.csv`, size: 459 B

### 3. **Architecture Diagram Update**
- Diagram updated to include new data enrichment join job using Glue.
- Left join between `Faculty Info` and `Preliminary Feedback` visualized.

### 4. **Glue Job Cost Analysis**
- Each summarization job's **execution time**, **job nodes used**, and **duration** were tracked:
  | Job                      | Executors | Nodes | Duration |
  |--------------------------|-----------|-------|----------|
  | Preliminary-Summarization | 2         | 10    | 1.50 min |
  | Faculty-Summarization     | 2         | 10    | 1.57 min |

---

## 📊 Glue Data Catalog Tables
- `faculty performance metrics` (confirmed schema):
  - `department` *(string)*
  - `avg_teachingscore_#0` *(double)*
  - `report_date_ltz` *(timestamp)*

---

## ✅ Key Learning Outcomes
- Practical implementation of **data enrichment** using AWS Glue joins.
- Validated **data lineage** from source to transformed output.
- Tracked **job performance** and resource utilization.
- Understood **Glue transformations** and S3 format targeting (CSV/Parquet).

---

## 🧠 Next Steps
- Build data validation pipelines using **AWS Athena**.
- Explore **partitioning strategies** to optimize Athena queries.
- Begin setting up **dashboard visualizations** (QuickSight/Power BI).

---

## 📸 Screenshot Highlights
- Glue Studio Join Flow → `Faculty-Preliminary`
- Updated System/User S3 folders → Output verification
- Catalog Table → `faculty performance metrics`
- Diagram view → join logic + output structure
- Cost dashboard for job resource tracking

---

> **Author:** Lavish  
> **Week:** 5/10  
> **Course:** Cloud Computing - AWS Cloud Foundations
