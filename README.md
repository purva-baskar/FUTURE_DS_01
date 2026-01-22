
# 📊 Superstore Sales Analysis Dashboard - Power BI

## 🚀 Project Context
Developed for the **Future Interns Data Science & Analytics Internship (Task 1)**, this project converts raw transactional data into a high-impact diagnostic tool. 

The goal was to move beyond static reporting and create a **Strategic Intelligence Hub**. This dashboard allows stakeholders to navigate from high-level financial health to granular operational details, facilitating proactive rather than reactive decision-making.


## 🎯 Learning Objectives
Through this project, I aimed to master the end-to-end Data Analysis lifecycle, specifically:
* **Data Modeling:** Building a relational "Star Schema" by connecting Fact and Dimension tables.
* **Semantic Layering:** Creating advanced DAX measures to track non-raw metrics like Profit Margins and Return Rates.
* **Business Storytelling:** Designing an interactive UI that prioritizes executive-level KPIs before drilling into granular details.
* **Diagnostic Analytics:** Using data to identify "The Why" behind sales trends and profitability gaps.

## 🖥️ Dashboard Preview
Below are the snapshots of the final interactive dashboard:
<img width="896" height="499" alt="image" src="https://github.com/user-attachments/assets/f80e2370-b91d-4ce5-9081-863c51ae3a9c" />


## 📖 Dashboard Explanation

* **KPI Cards:** Provides immediate visibility into Total Revenue ($2.3M), Net Profit ($286K), and total Order volume.
* **Monthly Performance Trends:** A line-graph comparison showing Revenue and Profit by month across years (2011–2014) to identify seasonal spikes.
* **Category Share:** A donut chart showing the revenue distribution, highlighting **Technology** as a primary driver.
* **Regional Revenue Distribution:** A geospatial bubble map identifying **California** and **New York** as market "Powerhouses."
* **Sales vs. Profit Scatter Plot:** A critical analysis showing which sub-categories have high sales volume but thin profit margins (e.g., Furniture).
* **Customer Segmentation:** Identifying the **Consumer Segment** as the most significant contributor to total revenue share.



## 🧠 Key Concepts & Learnings
During the development of this project, I applied several advanced analytical concepts:

* **DAX (Data Analysis Expressions):** Engineered custom measures such as:
    * `Return Rate = DIVIDE(COUNT(Returns[Order ID]), DISTINCTCOUNT(Orders[Order ID]))`
    * `AOV (Avg. Order Value) = DIVIDE([Total Sales], [Total Orders])`
* **Power Query ETL:** Handled data cleaning, restored deleted columns (Profit), and managed date hierarchies.
* **Data Visualization Standards:** Implemented a **Dark Mode** theme and "F-pattern" layout to optimize readability and user experience.
* **Relationship Management:** Managed 1-to-Many relationships between the primary `Orders` table and auxiliary `Returns`/`People` tables.



## 🏁 Conclusion
The **FUTURE_DS_01** dashboard serves as a bridge between raw data and strategic action. By centralizing disparate information into a single "Source of Truth," it allows managers to instantly identify loss-making territories and high-value product categories. This project underscores the role of Data Analytics in optimizing business performance and ensuring long-term profitability.

## Author
P.B.Purva  (Data analyst intern at Future Interns)



## 📂 Repository Structure
```text
FUTURE_DS_01/
│
├── Dashboard/
│   └── FutureInterns_DS_01.pbix
│
├── Dataset/
│   └── FutureInterns_DS_Dataset_01.csv
│
├── Screenshots/
│   ├── Dashboard.png
│
└── README.md
