# Customer Segmentation for Marketing Analysis

This project implements an end-to-end machine learning pipeline to group customers into distinct segments based on their demographic and purchasing behaviors. By leveraging **K-Means Clustering**, this analysis provides actionable insights to help businesses optimize targeted marketing strategies and improve customer engagement.

---

## Project Overview

Customer segmentation is essential for understanding the diverse needs of a consumer base. This project identifies specific customer **personas** using features such as income, spending patterns, and membership history.

---

## Key Objectives

- **Data Exploration:** Identify trends in customer age, gender, and category preferences  
- **Clustering:** Group 1,000 customers into meaningful segments using unsupervised learning  
- **Actionable Insights:** Define the characteristics of each cluster to guide marketing decisions  

---

## Dataset Description

The analysis uses a dataset of **1,000 entries** with the following features:

- **Age:** Customer's age  
- **Gender:** Male, Female, or Other  
- **Income:** Annual income level  
- **Spending Score:** Metric reflecting customer spending behavior  
- **Membership Years:** Duration of the customer's relationship with the brand  
- **Purchase Frequency:** How often the customer shops  
- **Preferred Category:** Electronics, Groceries, Clothing, Sports, or Home & Garden  
- **Last Purchase Amount:** Value of the most recent transaction  

---

## Methodology

### 1. Data Preprocessing
- Standardization of numerical features using **StandardScaler** to ensure equal weighting in K-Means  
- Encoding of categorical variables (**Gender**, **Preferred Category**) for model compatibility  

### 2. Optimal Cluster Determination
- Used the **Elbow Method** (via `KElbowVisualizer`) to identify the optimal number of clusters  
- Selected **k = 4**, balancing model simplicity and intra-cluster variance  

### 3. Clustering & Customer Profiles
The model successfully identified four distinct customer segments, including:

- **High-Value Frequent Shoppers:** High income, high spending scores, frequent purchases  
- **Niche Category Fans:** Customers with strong preferences for categories such as *Sports* or *Home & Garden*  

---

## Technologies Used

- **Python:** Core programming language  
- **Pandas & NumPy:** Data manipulation and numerical analysis  
- **Matplotlib & Seaborn:** Data visualization and heatmaps  
- **Scikit-learn:** K-Means clustering and preprocessing  
- **Yellowbrick:** Cluster evaluation and visualization  

---

## Installation and Setup

### Install Dependencies
Ensure Python is installed, then run:
```bash
  pip install -r requirements.txt
```
### Run the Analysis
```bash
  jupyter notebook "customer segmentation.ipynb"
```

## Conclusion

The analysis reveals that **purchase frequency** and **income** are the most significant differentiators among customers. By targeting the identified clusters with tailored marketing strategies—such as loyalty rewards for high-spending customers—businesses can significantly improve engagement and increase marketing ROI.

## Requirements

- Pandas  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Yellowbrick  
- Kaggle (for dataset download)  


