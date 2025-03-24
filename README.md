# 🏥 Hospital Emergency Room Analysis - Power BI Dashboard
## 📌 Project Overview
This Power BI project analyzes sales data for ... to provide actionable insights into various aspects of ... performance. The dashboard helps the ... track... performance across different aspects and time periods.
## ❓ Problem Statement
...

The goal is to analyze these aspects to **identify key ... and areas for improvement**.
## 🛠️ Skills Demonstrated
-	**Power BI** for data visualization, modeling, and analysis.
## 📊 Dataset Information
- Source: Excel file containing sales data.
- Key Columns:...

## 🔄 Data Transformation
To optimize performance and structure, **Power Query** was used to transform the raw dataset into a **star schema model**. The original dataset was broken down into:
-	**Fact Table**:
    -	Fact_Sales: ...   
-	After applying transformations in Power Query and loading the data into **Power BI Desktop**, two additional dimension tables were added to support **time intelligence calculations**:
    -	Dim_Date: Contains Date, DateKey, DayNo, and isWeekend fields for date-based analysis.
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
...

## 📌 Conclusion & Recommendations
...

## 🚀 How to Use This Dashboard
1.	Download the .pbix file from the repository.
2.	Open Power BI Desktop and load the file.
3.	Use filters and slicers to explore insights interactively.
___
🔗 For further improvements, feel free to fork this project and contribute! 🚀
