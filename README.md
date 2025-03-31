# 🏥 Hospital Emergency Room Analysis - Power BI Dashboard
## 📌 Project Overview
This Power BI project analyzes emergency room (ER) data to provide actionable insights into patients' visits, waiting time, and satisfaction. The dashboard helps hospital administrators and medical staff monitor ER performance, optimize resource allocation, and improve patient care by identifying trends in admissions, and peak visit periods.

## ❓ Problem Statement
The hospital's emergency room (ER) is experiencing challenges in patient admission management and operational efficiency. Key areas of concern include:
- **Patient Visit Trends** – Understanding daily, weekly, and seasonal fluctuations in ER visits.
- **Wait Time Management** – Analyzing the time patients spend before receiving treatment and its impact on patient satisfaction.
- **Demographic Insights**– Evaluating patient distribution by age, gender, and race to ensure equitable healthcare access.
- **Department Referrals** – Understanding which departments receive the most ER patients and the relationship with waiting time and satisfactions.
- **Peak Hours & Resource Allocation** – Identifying high-traffic periods to optimize staff scheduling and medical resource allocation.

The goal is to analyze these factors using a Power BI dashboard to improve ER efficiency, reduce waiting times, enhance resource planning, and ultimately provide better patient care. 🚑📊

## 🛠️ Skills Demonstrated
-	**Power BI** for data visualization, modeling, and analysis.
## 📊 Dataset Information
- Source: Excel file containing sales data.
- Key Columns:
    - date
    - patient_gender
    - patient_age
    - patient_sat_score
    - patient_race
    - patient_admin_flag
    - patient_waittime
    - department_referral

## 🔄 Data Transformation
To optimize performance and structure, **Power Query** was used to transform the raw dataset into a **star schema model**. The original dataset was broken down into:
-	**Fact Table**:
    -	Hospital ER: Contains transactional patients' visits including date, gender, age, satisfaction score, race, admin_flag, waittime and department referral.
-	After applying transformations in Power Query and loading the data into **Power BI Desktop**, two additional dimension tables were added to support **time intelligence calculations**:
    -	Dim_Date: Contains Date, DateKey, DayNo, Weekday, Quarter, and isWeekend fields for date-based analysis.
    -	Dim_Time: Includes Hour, Minute, Second, and Time fields to enable time-based insights.
    -	
## 📐 Data Modeling
Below is the **star schema model** and support tables used in this project:
 ![](images/Schema.PNG)
 
## 📈 Analysis & Visualizations
 ![](images/VisitOverview.PNG)
 
 ![](images/PatientOverview.PNG)
 
  ![](images/SatisfactionOverview.PNG)
  
The Power BI dashboard consists of various visual elements to display insights:
1. **Total Patients Analysis** - Card & Variation Display showing visits trends.
2. **Average Waiting Time Analysis** - Card & Variation Display showing waiting periods.
3. **Average Satisfaction Score Analysis** - Card & Variation Display illustrates ER performances.
4. **Total Patients by Admin Flag** - Pie Chart to show the proportion of patients administration.
5. **Total Patiens Trends (Year, Month, Day, Weekday, and Hours)** - Area Chart showing visits trends across different time scales.
6. **Total Patiens Distribution (Age, Race, Department Referral, Age Group)** - Bar Chart showing patients' demography.
7. **Relationship Between Average Waiting Time And Satisfaction Score** - Scatter Plot with mean lines to cluster visits by Department.
8. **Patients Satisfaction List View** - Table with custom star-rating visualisation for satisfaction scores.
9. **Dynamic Content for WeekDay and Hours Trends** - Field Parameter for more insights.
10. **Toggle Button for Split View (Line Chart) and Merge View (Matrix)** - Interactive options for better peak period spotting.
    
## 📌 Conclusion & Recommendations
1. **Resource Allocation:** Focus on staffing and resource optimization during peak months (Q2 and Q3) and peak hours (midday and midnight).
2. **Efficient Triage:** Improve triage and management systems to handle the high volume of non-referred patients and reduce waiting times.
3. **Age Group:** Patients aged 20-30 constitute the majority of visits, while those aged 70+ are the least represented. Resources and services should be tailored to meet the needs of younger patients, though attention to older adults should not be neglected.
4. **Monitor and Improve Satisfaction:** Ensure that departments with longer waiting times (Gastroenterology, Neurology, Physiotherapy) continue to provide high-quality service, while also working to reduce wait times in other departments without compromising care, and to promote the overal satisfaction score which is only above average (5.47/10)

## 🚀 How to Use This Dashboard
1.	Download the .pbix file from the repository.
2.	Open Power BI Desktop and load the file.
3.	Use filters and slicers to explore insights interactively.
___
🔗 For further improvements, feel free to fork this project and contribute! 🚀
