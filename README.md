# 📊 AI-Driven Sales Data Analytics & Anomaly Detection Dashboard

🚀 **Project Overview**
This project is an advanced, interactive Sales Analytics Dashboard developed in Microsoft Power BI. Unlike standard descriptive dashboards, this project focuses on **Diagnostic and Augmented Analytics** by leveraging Power BI's built-in Artificial Intelligence (AI) capabilities. It empowers stakeholders to not only see *what* happened but understand *why* it happened through automated insights, root-cause analysis, and anomaly detection.

---

## 🛠️️ Technical Challenges & Solutions

During the data modeling and dashboard development phase, several real-world technical challenges were addressed to ensure 100% data accuracy and optimal AI performance:

**1. Data Cleaning & Noise Reduction (Blank Row Issue)**
*   **Problem:** The raw dataset contained hidden empty rows and null values, which created a massive `(Blank)` category that distorted the Total Sales KPI (inflating it incorrectly) and skewed the bar charts.
*   **Solution:** Utilized **Power Query Editor** to systematically clean the data. Applied the `Remove Blank Rows` function and filtered out `(null)` values from the Category column, ensuring the AI engine processes only clean, valid transactions.

**2. Optimizing AI Model for Key Influencers**
*   **Problem:** Initially, the AI Key Influencers visual returned a "No influencers found" error. The visual was aggregating the entire dataset into a single sum, failing to analyze row-level transactional impact.
*   **Solution:** Reconfigured the visual's analytical engine. Changed the Analysis Type to `Continuous` and applied a `Don't summarize` rule to the Sales metric. This forced the AI to evaluate every individual transaction, successfully identifying the statistical drivers of high sales.

---

## 📈 Dashboard Pages & Visual Breakdown

This single-page, highly interactive dashboard contains 6 primary components, smoothly integrated for cross-filtering:

1. **Executive KPI Card (Total Sales):** 
   Provides an immediate high-level snapshot of the total revenue generated ($204K), acting as the baseline for all subsequent filtering.

2. **Sales by Category (Bar Chart):** 
   Compares revenue contribution across different product lines (Electronics, Furniture, Sports, Clothing, Food). It serves as a primary interactive slicer for the entire page.

3. **Sales Trend Over Time (Line Chart with AI Anomaly Detection):** 
   Tracks daily sales fluctuations. **AI Anomaly Detection** is enabled with custom sensitivity to automatically flag unexpected spikes or drops in sales (indicated by grey markers), allowing immediate investigation into unusual market behaviors.

4. **Sales Breakdown by Factors (AI Decomposition Tree):** 
   An interactive root-cause analysis tool. It allows users to dynamically break down Total Sales across multiple dimensions (`Region` ➔ `Category` ➔ `Product`). The AI automatically determines the next highest-value split, instantly revealing that the 'East' region and 'Electronics' category are the primary contributors.

5. **Key Drivers of Sales (AI Key Influencers):** 
   Uses machine learning to analyze the dataset and identify which specific factors drive sales increases. For example, it statistically proves that when the Category is *Electronics* or the Product is *Phone*, the average sales significantly increase compared to other items.

6. **Automated Insights (Smart Narrative):** 
   An AI-generated text box that dynamically writes a natural language summary of the dashboard. As the user clicks on different charts, this narrative auto-updates to provide instant, readable takeaways without requiring manual data interpretation.

---

## 📂 Repository Contents

*   **`AI-Driven Sales Data Analytics & Anomaly Detection Dashboard.pbix`** : The fully functional Power BI dashboard containing the data model, AI visuals, and interactive charts.
*   **`AI-Driven Sales Data Analytics & Anomaly Detection Dashboard.xlsx`** : The raw dataset used for this project.
*   **`AI-Driven Sales Data Analytics & Anomaly Detection Dashboard.jpg`** : A high-resolution image preview of the completed dashboard.
*   **`AI-Driven Sales Data Analytics & Anomaly Detection Dashboard.pdf`** : A static PDF export of the complete report for quick executive review.

---

## 👨‍💻 Author

**Bayzid Mostak**<br>
*Data Analyst & Visualization Expert*

*   [LinkedIn] https://www.linkedin.com/in/bayzid-mostak-data-analyst/
*   [GitHub] https://github.com/TusharAlBayzid
*   Note: Download the `.pbix` file and open it in Power BI Desktop to experience the fully interactive cross-filtering capabilities of this dashboard.
