# 🛒 Online Retail Customer Segmentation Report

## 📌 Project Overview

This project focuses on **customer segmentation** using clustering techniques applied to an **Online Retail** dataset. By analyzing customer transactions, we identify distinct groups of customers based on **Recency, Frequency, and Monetary (RFM)** behavior, using machine learning models such as **K-Means** and **DBSCAN**.

## 🎯 Objectives

- Prepare and clean the data.
- Perform exploratory data analysis (EDA).
- Extract RFM features.
- Apply clustering algorithms (K-Means & DBSCAN).
- Evaluate and visualize clustering results.
- Export final customer segmentation dataset for business intelligence use.

---

## 📁 Dataset

**Original File:** `Online Retail.xlsx`

**Final Cleaned File (with RFM + Clustering):** `final_data_with_all_clusters.xlsx`

**BI Dashboard File:** `Online Retail Report.pbix`

**Main Columns Used:**

- `InvoiceNo`
- `StockCode`
- `Description`
- `Quantity`
- `InvoiceDate`
- `UnitPrice`
- `CustomerID`
- `Country`

---

## 🔧 Steps & Methodology

### 1. 📚 Importing Libraries

Used essential libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`, `yellowbrick`.

---

### 2. 🧼 Data Preparation

- Loaded data using `pd.read_excel`.
- Displayed basic stats, structure, and data types.
- Checked and removed missing and duplicate values.
- Removed rows with negative or zero `Quantity` or `UnitPrice`.

---

### 3. ✨ Feature Engineering

- Created a new column `TotalPrice = Quantity * UnitPrice`.
- Computed **Recency**, **Frequency**, and **Monetary** values for each customer.
- Applied **StandardScaler** to normalize RFM features.

---

### 4. 📊 Exploratory Data Analysis (EDA)

- **Monthly Sales Trend**
- **Top Countries by Sales & Invoice Count**
- **Top Selling Products**
- **Distribution of RFM metrics**
- **Correlation Heatmap**
- **Top Customers by Frequency, Monetary, Recency**

---

### 5. 🤖 Clustering Models

#### 📌 K-Means Clustering

- Used **Elbow Method** and **Silhouette Score** to find optimal `k`.
- Applied model with `k = 4`.
- Assigned cluster labels to customers.
- Visualized clusters using boxplots.

#### 📌 DBSCAN Clustering

- Used K-Distance Graph to choose `eps`.
- Applied DBSCAN and visualized clusters using scatter plot.

---

### 📈 Cluster Evaluation Summary

Both clustering techniques were evaluated by computing average **Recency**, **Frequency**, and **Monetary** values per cluster. Insights were drawn for business segmentation and potential marketing strategies.

---

### 📌 VIP Customers

- Customers in **Cluster 2,3 (K-Means)** were considered **important customers** based on high Frequency & Monetary scores.
- DBSCAN cluster `-1` was used to detect **outlier/high-value** customers.

---

## 📦 Deliverables

- ✅ Cleaned Dataset with Features & Clusters (`final_data_with_all_clusters.xlsx`)
- ✅ Power BI Dashboard (`Online Retail Report.pbix`)
- ✅ Full Code in Python (Jupyter Notebook / .py)
- ✅ Visualizations for all major steps
- ✅ Summary Statistics for each cluster

---

## 📊 BI Dashboard (Power BI)

The final cleaned dataset was used to build a fully interactive dashboard in **Power BI**, enabling:

- Customer profile exploration
- Cluster filtering
- RFM distributions
- Time-based sales trends
- Country-wise performance

---

## 🛠 Tools & Technologies

- Python
- Pandas, NumPy, Seaborn, Matplotlib
- Scikit-learn, Yellowbrick
- DBSCAN, KMeans
- Jupyter Notebook
- Power BI

---

## 📎 Author

**Mohamed [Your Last Name]**

- 📧 Email: [mohamedkhlawy153@gmail.com]
- 🔗 Linkedin: [https://www.linkedin.com/in/mohamed-mahmoud-17030b2a3/]
- 🧠 Project Type: Customer Segmentation | Machine Learning | BI

---

## 💡 Future Work

- Apply deep learning for pattern recognition.
- Build a recommendation engine based on clusters.
- Integrate real-time customer updates via APIs.
