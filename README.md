# 🧠 Census Analytics SQL – Insights from India’s Census Data

This project explores **India’s census data at the district level** using SQL to uncover key demographic and social insights. It demonstrates how raw datasets can be transformed into **actionable knowledge** using a wide range of **basic to advanced SQL queries**.

---

## 📌 Project Highlights

This analysis dives deep into India's demographics to:

- Estimate **previous census population** using growth rates.
- Calculate **literacy and illiteracy counts** by district and state.
- Derive **male and female population** using sex ratios.
- Rank districts using **window functions** (e.g., `RANK()`).
- Compute **population density** (people per square km).
- Identify **top 3 literate districts** in each state.

The project reflects a strong grasp of SQL for real-world data analysis, with clear logic, structured queries, and a focus on clarity and insight.

---

## 🧠 SQL Concepts Used

Throughout the project, the following SQL concepts were applied:

- **Table Joins** and **Subqueries**
- **Aggregate Functions** (`SUM`, `ROUND`, etc.)
- **Window Functions** (`RANK() OVER` for ranking)
- **Derived Fields** and Custom Calculations
- **Grouping**, **Filtering**, and **Ordering Logic**

The queries range from simple `SELECT` statements to complex nested logic, showcasing both foundational and advanced SQL skills.

---

## 🗃️ Database Schema

Two tables were used and joined on the `District` field for comprehensive analysis:

### 🔹 `data1` (Demographic Metrics)

| Column     | Description                     |
|------------|---------------------------------|
| State      | Name of the state               |
| District   | Name of the district            |
| Sex_Ratio  | Female-to-male ratio            |
| Literacy   | Literacy rate (%)               |
| Growth     | Population growth rate (%)      |

### 🔹 `data2` (Population & Area)

| Column     | Description                     |
|------------|---------------------------------|
| District   | District name                   |
| State      | State name                      |
| Population | Total population                |
| Area_Km2   | Area in square kilometers       |

---

## 📊 Sample Calculation Logic: Gender Breakdown

Using the sex ratio, we estimate male and female population as:

- **Males** = Population / (1 + Sex_Ratio)
- **Females** = Population - Males

This approach allows for estimating gender distribution even when only aggregate data is available.

---

## 🧾 Files Included

- `india_census_analysis.sql` — SQL script containing all queries and logic
- `README.md` — This documentation file
- `data1.csv` & `data2.csv` — (Optional) Source datasets for local use

---

## 💻 How to Run

1. Clone the repository to your local system.
2. Import `data1.csv` and `data2.csv` into a SQL Server database (e.g., named `project`).
3. Open the `india_census_analysis.sql` file using SSMS or any SQL editor.
4. Run the queries to view and explore the insights.

---

## 🤝 Connect With Me

I'm open to feedback, learning opportunities, and collaborations!

- **Email**: [abhijeetpunia03@gmail.com](mailto:abhijeetpunia03@gmail.com)

---

⭐ If you find this project helpful or insightful, consider giving it a **star** on GitHub!

