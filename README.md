# Job Search and Application Tracker

## Project Overview
A **Microsoft Power Platform** solution that streamlines job searching and application tracking. The system integrates **Power Apps, Power Automate, SharePoint, and Power BI** to provide a seamless experience for users. It fetches real-time job listings from the **Jooble API (REST API integration)**, allows users to save and track applications in **SharePoint Lists**, and automates status updates using **Power Automate**. The application also connects to **Power BI via a Streaming Data API**, offering real-time analytics on job applications. Designed with **security and access control**, this project showcases expertise in **low-code development, automation, and data visualization**..


## **Business Use Case:**  

### **Problem Statement**  
Since completing my master's thesis in January 2025, I have applied to numerous job openings and had a couple of interviews but I have faced challenges in effectively managing my job applications, tracking application statuses, remembering follow-up dates, and identifying which job roles or industries yield more interview opportunities. Interestingly from my research, I found that **59% of job seekers find the job search process as time-consuming as a full-time job**, and **77% lose track of crucial follow-up opportunities**, leading to missed chances and inefficiencies as stated by an Article published by ResponseSource. Therefore, I decided to develop a solution that streamlines application tracking and provides insights into job search performance.

Job seekers often struggle with:  
- Tracking their job applications and follow-ups efficiently.  
- Identifying patterns in their job search performance.  

### **Solution**  
This **Microsoft Power Platform** solution integrates **Power Apps, Power Automate, SharePoint, and Power BI** to:  
- Search for jobs in real-time via Jooble API within Power Apps.  
- Save and track applications in SharePoint Lists.  
- Automate status updates using Power Automate.  
- Visualize job application trends in Power BI, showing which roles they are more likely to get a job in.  

### **Business Benefits**  
✅ Streamlines job tracking and reduces manual effort.  
✅ Helps users focus on high-success job titles based on data insights.  
✅ Provides real-time performance analytics to refine job search strategy.  

In general, this solution empowers job seekers with data-driven insights, allowing them to optimize their job search efforts effectively


## Solution Architecture
![Architecture-1](https://github.com/Godwin-will/JobSearchandApplicationTracker/blob/main/jobsearcharchi2.png)


## Data Flow

1. **Data Extraction:** Power Automate extracts real-time job listings from the **Jooble API (REST API integration)** based on user input in **Power Apps**.  
2. **Data Processing:** Extracted job data (Job Title, Location, and Job Link) is processed and formatted within **Power Automate** before being sent to **Power Apps** for display.  
3. **Data Storage:** Users save job applications via a form in **Power Apps**, and the details (job title, company, application status, etc.) are stored in **SharePoint Lists** for tracking.  
4. **Data Automation:** Power Automate updates and modifies job application statuses dynamically in **SharePoint Lists**, ensuring real-time data consistency.  
5. **Data Loading:** SharePoint List data is connected to **Power BI** via a Streaming Data API for continuous updates and real-time analytics.  
6. **Data Visualization:** Power BI generates interactive dashboards to provide insights into application status, success rates, and job search trends.


## Technologies Used  
- **Power Apps:** Provides a user-friendly interface for job searching and application tracking.  
- **Power Automate:** Automates job data extraction, processing, and updates from Jooble API to Power Apps and SharePoint.  
- **SharePoint Lists:** Stores job application details, statuses, and updates for easy access and tracking.  
- **REST API (Jooble API):** Fetches real-time job listings based on user input in Power Apps.  
- **Power BI:** Connects to SharePoint Lists via a Streaming Data API for real-time job application analytics and visualization.
  

## **Key Features**  

🔹 **Job Search Integration** – Search for real-time job listings using the **Jooble API** directly within Power Apps.  
🔹 **Application Tracking** – Save job applications in **SharePoint Lists** and update statuses dynamically.  
🔹 **Automated Updates** – Use **Power Automate** to modify and manage job application statuses automatically.  
🔹 **Real-Time Data Visualization** – **Power BI dashboards** provide insights into job search performance, including rejection vs. interview trends.  
🔹 **User-Friendly Interface** – Intuitive **Power Apps** UI allows seamless job search, tracking, and management.  
🔹 **Data-Driven Decision Making** – Helps job seekers focus on job titles with higher success rates based on application outcomes.



![Image](https://github.com/user-attachments/assets/7d469a9b-e6cd-44a0-b328-11b9cf2a5cce)






























## ETL Pipeline
The ETL pipeline consists of the following key tasks:
1. **Data Extraction:**
   - Extract data from the Spotify blob storage using Azure Data Factory.
2. **Data Transformation:**
   - Utilize Azure Databricks to perform necessary transformations on the Spotify data.
3. **Data Loading:**
   - Store the processed data in Azure Data Lake Storage for flexibility.
4. **Data Ingestion:**
   - Ingest data from Data Lake Storage to SQL Database for structured storage.
5. **Data Visualization:**
   - Connect Power BI to the SQL database for interactive data visualization.

![Code-1](https://github.com/kingsley-123/Spotify-ETL-/assets/63650573/fbd48c88-14bd-4cbd-b8c6-c721f98003f4)
![Code-2](https://github.com/kingsley-123/Spotify-ETL-/assets/63650573/2f4721d4-bb3c-4923-9991-6d42bdf10ccb)
![Code-3](https://github.com/kingsley-123/Spotify-ETL-/assets/63650573/7da95090-cd9d-4b73-ad7c-1e528cf89cff)


## Development Setup
To set up and run the data pipeline locally, follow these steps:
- Provision necessary Azure resources, including Data Factory, Databricks, Data Lake Storage, and SQL Database.
- Configure connections and credentials for each component.
- Define required environment variables or configuration files.
- Execute the pipeline using Azure Data Factory triggers or manual execution.

  
## Spotify Visualization 
![Spotify Report-1](https://github.com/kingsley-123/Spotify-ETL-/assets/63650573/40d8290a-20b5-430b-aaea-46181dd1188c)


