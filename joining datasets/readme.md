
# Week 5 Cloud Portfolio - README.md

## ✅ Overview
In Week 5, the focus was on **joining datasets**, **data enrichment**, and **job optimization** using AWS Glue Studio. We built and executed the `Faculty-Preliminary` join job, monitored its output in S3, and validated data transformation and storage. 

---

## 📁 Project Structure
```
aws-cloud-portfolio/
├── week5/
│   ├── glue-jobs/
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
![image5](https://github.com/user-attachments/assets/5227ae97-d255-40de-9f35-48e5cad26926)
![image4](https://github.com/user-attachments/assets/1261534f-6e68-4fa3-9814-aa03d9e23502)
![image3](https://github.com/user-attachments/assets/9c4af85a-60a6-420b-a35f-a5ed80ecf443)
![image2](https://github.com/user-attachments/assets/75115e81-823b-4f24-b981-05d1c5ab541d)
![image1](https://github.com/user-attachments/assets/f3b69c82-8e2d-4b5e-9a8f-1b725fb40399)

---

> **Author:** Lavish  
> **Week:** 5/10  
> **Course:** Cloud Computing - AWS Cloud Foundations
