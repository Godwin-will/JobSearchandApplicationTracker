# Job Search and Application Tracker

## Project Overview
<p align="justify">
A <b>Microsoft Power Platform</b> solution that streamlines job searching and application tracking. The system integrates <b>Power Apps, Power Automate, SharePoint, and Power BI</b> to provide a seamless experience for users. It fetches real-time job listings from the <b>Jooble API (REST API integration)</b>, allows users to save and track applications in <b>SharePoint Lists</b>, and automates status updates using <b>Power Automate</b>. The application also connects to <b>Power BI via a Streaming Data API</b>, offering real-time analytics on job applications. Designed with <b>security and access control</b>, this project showcases expertise in <b>low-code development, automation, and data visualization</b>.
</p>


## **Business Use Case:**  

### **Problem Statement**  
<p align="justify">
Since completing my master's thesis in January 2025, I have applied to numerous job openings and had a couple of interviews but I have faced challenges in effectively managing my job applications, tracking application statuses, remembering follow-up dates, and identifying which job roles or industries yielded me more interview opportunities. Interestingly from my research, I found that <b>59% of job seekers find the job search process as time-consuming as a full-time job</b>, and <b>77% lose track of crucial follow-up opportunities</b>, leading to missed chances and inefficiencies as stated by an Article published by ResponseSource. Therefore, I decided to develop a solution that streamlines application tracking and provides insights into job search performance.
</p>


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


## **User Interface**  

The Job Search & Application Tracker is designed with a user-friendly interface, allowing job seekers to seamlessly search for jobs, track applications, and gain insights into their job search performance.  

#### **1. Home Screen (Job Search Page)**  
- The search bar allows users to input job titles and locations.  
- A search button triggers the Power Automate flow, fetching job listings via the Jooble API.  
- The results are displayed in a list format, showing:  
  - **Job Title**  
  - **Company Name**  
  - **Location**  
  - A **link button (arrow icon)** that directs users to the job application page.  


![Image](https://github.com/user-attachments/assets/a21749c9-6f2b-43ec-89ed-feb8f792edeb)

##### Power Automate Flow
![Image](https://github.com/user-attachments/assets/c244ceb2-fa71-4a5b-ba27-43bcb520b8b0)


#### **2. Save Application Page**  
- Users can save job applications they have applied to using a custom form.  
- The form captures key details such as:  
  - **Job Title**  
  - **Company Name**  
  - **Application Date**  
  - **Application Status (e.g., Applied, Interview, Rejected, Offer Received)**  
- Saved job applications are stored in **SharePoint Lists** for easy tracking.  
- Users can update the application status as they progress in their job search.  


![Image](https://github.com/user-attachments/assets/dafc2873-a798-496d-816e-e1c9c9cc9f98)

##### Power Automate Flow
![Image](https://github.com/user-attachments/assets/09fee5e9-c678-4007-98cc-73d3ed2af5a0)

##### SharePoint Updated List
![Image](https://github.com/user-attachments/assets/2fc2f1c7-0537-4fc5-a9ed-5babf1be4e48)


#### **3. Insights Dashboard**  
- Users can view real-time analytics on their job search performance.  
- The dashboard is powered by **Power BI**, connected to the SharePoint list via a **streaming data API.**  
- Key insights include:  
  - **Number of applications sent over time**  
  - **Job roles and industries where the user gets more interviews**  
  - **Application success rate (Interviews & Offers vs. Rejections)**  
  - **Follow-up reminders based on pending applications**  
- The goal is to help users optimize their job search strategy by identifying trends in their applications.  


