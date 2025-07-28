# 🛍️ Online Retail Data Analysis Project

This project focuses on exploring, cleaning, and analyzing a real-world e-commerce dataset from a UK-based online retail store. Using data science techniques such as clustering, product analysis, and customer segmentation, we extract insights to support business strategies like marketing, inventory planning, and recommendation systems.

---

## 📦 Dataset Description

The dataset contains transactional data for one year (Dec 2010 – Dec 2011) and includes:

- **InvoiceNo**: Unique identifier for each transaction  
- **StockCode**: Unique product/item code  
- **Description**: Name of the product  
- **Quantity**: Number of items purchased  
- **InvoiceDate**: Date and time of the purchase  
- **UnitPrice**: Price per item (in GBP)  
- **CustomerID**: Unique customer ID (some are missing)  
- **Country**: Country of the customer  

Dataset Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Online+Retail)

---

## ❓ Problem Statement

The project aims to derive actionable insights from raw transaction data to support business decision-making. The main objectives include:

- Identifying high-value and loyal customers using clustering  
- Discovering top-selling and underperforming products  
- Performing market basket analysis to uncover product combinations  
- Analyzing country-wise and seasonal trends in purchases  
- Creating a basic recommendation system using product co-occurrence  
- Enhancing customer targeting and inventory planning  

---

## 🧹 Data Preprocessing

Key cleaning steps include:

- Handling missing values (`CustomerID`, `Description`)  
- Removing duplicate records  
- Filtering out canceled orders (InvoiceNo starting with 'C')  
- Removing rows with negative or zero `Quantity` and `UnitPrice`  
- Feature engineering (`TotalPrice = Quantity × UnitPrice`, `Month`, `Day`)  

---

## 📊 Exploratory Data Analysis

- Country-wise sales distribution  
- Top 10 most sold and most returned products  
- Revenue trends over months  
- Quantity and unit price analysis  
- Customer purchase frequency distribution  

---

## 📈 Machine Learning Models

###  **Customer Segmentation (Clustering)**

We applied **both K-Means Clustering** and **Agglomerative Hierarchical Clustering** to segment customers based on features like Recency, Frequency, and Monetary value (RFM). After evaluating silhouette scores and dendrograms, **4 clusters** were found to be optimal, representing distinct groups such as high-value customers, frequent buyers, occasional shoppers, and low-engagement users.

- **K-Means**: Used to partition customers into 4 distinct groups using Euclidean distance and elbow method  
- **Agglomerative Clustering**: Applied to cross-validate and compare results using hierarchical linkage methods  

## ▶️ How to Run

Clone this repository:
```bash
git clone https://github.com/kanishka2985/Online-Retail-Clustering-Project/tree/main.git
cd Online-Retail-Clustering-Project
```



