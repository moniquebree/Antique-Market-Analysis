# Project 1: Production Efficiency Dashboard

## 1. Project Objective
The goal of this analysis was to identify the key drivers of cost and time in a production dataset. I used Python for data cleaning and Power BI to create an interactive "Executive Dashboard" that reveals insights on department efficiency, item costs, and monthly trends.

## 2. Tools Used
* **Python (Jupyter Notebook):** Used for all data cleaning and transformation.
* **Pandas:** The primary library used to clean, aggregate, and analyze the data.
* **Power BI:** Used for the final, interactive dashboard and DAX measure creation.

## 3. The Process
1.  **Data Cleaning (Python):** Loaded the raw CSV. Discovered and rectified hidden errors in column names (like `\n` characters, ` ` extra spaces) and in the data itself (e.g., 'machine' to 'Machine').
2.  **Analysis (Python):** Performed three key analyses: Departmental, Item, and Time-Series.
3.  **Dashboard (Power BI):**
    * Imported the *master clean* dataset.
    * Created new **DAX measures** to calculate `Total Cost` (Direct + Overhead) and `Cost per Hour` (Efficiency).
    * Built a single, interactive "Executive Dashboard" page with KPIs, slicers, and a 2x2 grid answering the key business questions (When, Where, Why, and What).

## 4. Key Findings (The Story)
* **Finding 1: The '80/20' Cost Drivers.** The analysis revealed that just two departments, **Painting ($12.76M)** and **Assembly ($9.46M)**, are the primary cost centers, driving a combined **78% of all production costs**.

* **Finding 2: The Efficiency Paradox.** The dashboard's 'Cost per Hour' measure showed that the most *costly* department (Painting) is not the least *efficient*. The **'Curtains' department ($66.94/hr)** has the highest cost per hour, making it the least efficient, while **'Control & Packing' ($40.63/hr)** is the most efficient.

* **Finding 3: Key Trends & Items.** Costs are not flat; they spike significantly in **March** and **December**, suggesting seasonal pressure. The single largest item driving these costs is **'Ceiling'**, which represents a major target for any future cost-saving investigation.

## 5. Next Steps
The next step would be to acquire sales revenue data to measure true profitability per item.
