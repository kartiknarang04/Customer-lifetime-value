# Customer Lifetime Value (CLV) Prediction & Behavioral Segmentation

This project performs a comprehensive data analysis of an e-commerce transactional dataset to **predict customer lifetime value (CLV)** and **segment the customer base** based on purchasing behavior.  
It leverages advanced analytical and machine learning techniques to provide actionable insights for **business strategy, marketing, and customer retention**.

---

## 📌 Project Objectives
- **Predict Customer Lifetime Value (CLV):** Build a predictive model to forecast the future revenue a customer is expected to generate.  
- **Segment the Customer Base:** Use unsupervised learning to identify distinct customer groups based on their behavioral patterns.  
- **Conduct Cohort Analysis:** Analyze customer retention and churn over their lifetime to understand time-based behavioral trends.  
- **Deliver Actionable Insights:** Translate complex data findings into clear, strategic recommendations for improving business outcomes.  

---

## 📊 Dataset
The analysis is performed on a public **e-commerce transactional dataset** containing ~540,000 records.  

**Key Columns:**
- `InvoiceNo` → Unique identifier for each transaction  
- `StockCode` → Unique identifier for each product  
- `Description` → Product name  
- `Quantity` → Quantity purchased  
- `InvoiceDate` → Date and time of the transaction  
- `UnitPrice` → Price per unit  
- `CustomerID` → Unique identifier for each customer  
- `Country` → Country of the customer  

---

## 🛠 Methodology

### 1. Data Preprocessing & EDA
- Cleaned raw data (handled missing values, outliers).  
- Performed exploratory analysis to identify sales trends, top-selling products, and customer distribution.  

### 2. Feature Engineering
Created a **rich customer profile** beyond basic RFM:  
- **Recency:** Days since last purchase  
- **Frequency:** Total number of unique purchases  
- **Monetary Value:** Total spend  
- **Average Order Value (AOV):** Average spend per transaction  
- **Purchase Interval:** Avg. time between purchases (days)  
- **Tenure:** Total time active (days)  

### 3. Customer Lifetime Value (CLV) Prediction
- Developed a **regression model** trained on historical data to predict CLV.  
- Evaluated using **Root Mean Squared Error (RMSE)**.  

### 4. Customer Segmentation
- Applied **K-Means Clustering** on engineered features.  
- Determined optimal clusters with the **Elbow Method**.  
- Resulting segments:  
  - 🏆 **Champions:** High-spending, frequent, recently active  
  - ⚠️ **At-Risk:** Previously valuable but inactive  
  - 🌱 **New Customers:** Recently acquired, high potential  

### 5. Cohort Analysis
- Grouped customers by **month of first purchase**.  
- Tracked:  
  - **Retention Rate** (returning customers %)  
  - **Revenue Growth** (lifetime spend trends)  
  - **Churn Rate** (drop-off points)  

---

## 📈 Key Findings & Business Insights
- A large portion of customers are **one-time buyers** → opportunity for re-engagement campaigns.  
- **Champions segment**, though small, contributes disproportionately to revenue → target for loyalty programs.  
- Retention drops sharply after **3 months** → need for stronger post-purchase engagement.  
- Predictive CLV model identifies **future high-value customers early** → enables proactive marketing.  

---

## 🧑‍💻 Technologies Used
- **Python**  
- **Pandas** → Data manipulation  
- **NumPy** → Numerical operations  
- **Scikit-learn** → Machine learning (Regression, Clustering)  
- **Matplotlib / Seaborn** → Data visualization  

