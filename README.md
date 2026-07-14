## 📊 Kickstarter Crowdfunding Projects Analysis — Power BI Dashboard

## 📌 Project Summary

A comprehensive Power BI analysis of Kickstarter crowdfunding projects, examining success rates, failure patterns, live project performance, country-level fundraising, creator categories, and pledge trends. This dashboard transforms raw Kickstarter data into actionable insights that help creators understand what drives campaign success.


## 📝 Project Overview

This project focuses on analyzing Kickstarter crowdfunding data to uncover key trends, success drivers, and failure patterns across different categories, countries, time periods, and creators.



## The dashboard provides:

Success, Failure, and Live project KPIs

Country-wise funding distribution

Category-wise pledge and goal analysis

Creator-level performance insights

Monthly funding trends

Goal range failure analysis

Interactive filtering for deeper exploration

This project demonstrates strong skills in Power BI, DAX, data modeling, data cleaning, and storytelling with data.




## 🎯 Problem Statement

Kickstarter has thousands of crowdfunding campaigns, but creators struggle to understand:

Why certain campaigns succeed or fail

Which categories perform best

How pledge amounts differ by country

What funding goals lead to higher chances of success

How creator reputation impacts results

Seasonal or monthly patterns in fundraising

This project solves these problems by providing an interactive dashboard with clear KPIs and insights.




## 🛠 Tools & Technologies
Tool	Purpose
Power BI Desktop	Dashboard creation, modeling, DAX calculations
Power Query (M language)	Cleaning, transforming datasets
Excel / CSV	Source dataset
DAX	Metrics, KPIs & calculated measures
Google Drive / GitHub	Storing dataset & PBIX file
🔧 Data Cleaning & Preparation




## Performed using Power Query:

✔ Removed duplicates
✔ Split and transformed columns
✔ Fixed inconsistent naming
✔ Filtered invalid entries
✔ Standardized date formats
✔ Converted currencies & numeric formatting
✔ Created proper data types for:

Date

Category

Country

Pledge amount

Goal amount

The final dataset was loaded into a star-schema model for better DAX performance.





## 📐 DAX Measures Used

Below are key measures included in the project:

Overall Successful % =
DIVIDE(
    CALCULATE(COUNTROWS('Table'), 'Table'[state] = "successful"),
    COUNTROWS('Table')
)

Overall Failed % =
DIVIDE(
    CALCULATE(COUNTROWS('Table'), 'Table'[state] = "failed"),
    COUNTROWS('Table')
)

Total Pledged = SUM('Table'[pledged])
Total Goal = SUM('Table'[goal])

Success % by Category =
DIVIDE(
    CALCULATE(COUNTROWS('Table'), 'Table'[state] = "successful"),
    CALCULATE(COUNTROWS('Table'))
)


Additional measures:

Monthly pledged amount

Goal range distribution

Country-wise pledged total

Creator-wise pledge comparison





## 📊 Dashboards Preview

🔹 Overall Kickstarter Dashboard
<img width="1182" height="666" alt="Screenshot 2025-10-29 104056" src="https://github.com/user-attachments/assets/731e9f58-285c-4323-9873-1cc5d73bcef3" />

🔹 Successful Projects Dashboard
<img width="1178" height="662" alt="Screenshot 2025-10-29 104108" src="https://github.com/user-attachments/assets/4c35b85f-e059-49fb-abdd-b79cb2567a35" />

🔹 Failed Projects Dashboard
<img width="1183" height="664" alt="Screenshot 2025-10-29 104124" src="https://github.com/user-attachments/assets/9eb2fd9b-3917-4cbe-b0eb-a85c39af8b35" />

🔹 Live Projects Dashboard
<img width="1181" height="665" alt="Screenshot 2025-10-29 104138" src="https://github.com/user-attachments/assets/0e662715-903b-42ba-9b4d-558a754e59bd" />





## ▶️ How to Run This Project?

1. Download the Power BI File (.pbix)

➡️ https://drive.google.com/file/d/1YQ65aORetZ6_uhPqxHKBiVpvPWmSjaXx/view?usp=sharing

2. Open in Power BI Desktop

Go to File → Open → Select .pbix file

3. Interact with Dashboard

Use slicers and filters to explore:

Categories

Creators

Countries

Time periods

Goal ranges





## 💡 Key Insights
✔ Success Rate: 38.35%

A significant number of projects do not reach their goals.

✔ Failure Rate: 51.45%

High failure rate indicates poor goal planning and lack of understanding of backer behavior.

✔ Top Categories by Funds Raised

Product Design

Video Games

Animation

Gadgets

✔ Top Creators by Funding

Creators with repeated successful campaigns generate higher pledge amounts.

✔ Country-Level Funding

The US dominates crowdfunding, contributing the highest pledged amount.

✔ Goal Range Failure

Projects with very high goals (2000+ units) have the highest failure percentage.

✔ Monthly Funding Trends

December and May show the highest pledge activity.






### 🏁 Results & Conclusion

The Power BI dashboard clearly shows:

Realistic, lower goals result in higher success.

Certain categories consistently outperform others.

The US contributes most of the global crowdfunding value.

Seasonality plays a major role in pledge activity.

Creator reputation improves campaign success.

This dashboard enables creators to make data-driven decisions before launching campaigns.





## 🚀 Future Work

✔ Add prediction models for success probability
✔ Add time-series forecasting for pledge amounts
✔ Enhance data with social media engagement metrics
✔ Include sentiment analysis from campaign descriptions
✔ Add category-based benchmarking





## 👤 Author & Contact

## Name: Athnash Kandulna
Email: athnash2003@gmail.com
LinkedIn: www.linkedin.com/in/athnash-kandulna-0687a3274
GitHub: https://github.com/Athnash/Athnash
