# Customer Segmentation Analysis

## About the Project

In this project, I worked on customer segmentation using Python and Machine Learning.

The main aim of this project is to divide customers into different groups based on their purchasing behaviour. This helps to understand which customers are regular, high-value, frequent or at risk of becoming inactive.

## Dataset

The dataset contains customer purchase information.

Some of the important columns used are:

- Customer_ID
- Date
- Age
- Gender
- City
- Product_Category
- Unit_Price
- Quantity
- Total_Amount
- Payment_Method
- Is_Returning_Customer
- Customer_Rating

The dataset contains **17,049 rows and 18 columns**.

Before starting the analysis, I checked the dataset for missing values, duplicate rows and data types.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## What I Did

### 1. Data Inspection

First, I loaded the dataset and checked:

- Number of rows and columns
- Column names
- Data types
- Missing values
- Duplicate records

There were no missing values or duplicate rows in the dataset.

### 2. RFM Analysis

I used RFM analysis to understand customer behaviour.

- **Recency** – How recently the customer made a purchase
- **Frequency** – How many times the customer purchased
- **Monetary** – How much the customer spent

These three features were used for customer segmentation.

### 3. Feature Scaling

Since Recency, Frequency and Monetary have different ranges, I used `StandardScaler` to standardise the values before applying clustering.

### 4. Elbow Method

I used the Elbow Method to find a suitable number of clusters.

The graph showed that **4 clusters** were suitable for this analysis.

### 5. K-Means Clustering

I applied the K-Means clustering algorithm and divided the customers into **4 different clusters**.

### 6. Cluster Analysis

I analysed the average Recency, Frequency and Monetary values for each cluster.

The clusters were interpreted as:

- **Cluster 0 – Regular Customers**
- **Cluster 1 – High-Value Customers**
- **Cluster 2 – At-Risk Customers**
- **Cluster 3 – Frequent Customers**

### 7. Visualisation

I created different scatter plots to understand the customer groups:

- Recency vs Monetary
- Recency vs Frequency
- Frequency vs Monetary

I also created a bar chart showing the number of customers in each cluster.

## Key Insights

- Cluster 0 contains the largest number of customers and has moderate purchasing behaviour.
- Cluster 1 has fewer customers but has the highest monetary value and high purchase frequency.
- Cluster 2 has high recency and low purchase frequency, so these customers may be at risk of becoming inactive.
- Cluster 3 has high purchase frequency and relatively recent purchases, but their spending is lower than Cluster 1.

## Marketing Recommendations

- Give loyalty rewards and exclusive offers to high-value customers.
- Use discounts and personalised offers to bring back at-risk customers.
- Use bundle offers and cross-selling for frequent customers.
- Use personalised recommendations and promotions for regular customers.

## Conclusion

This project helped me understand how customer segmentation can be done using RFM analysis and K-Means clustering.

Instead of treating all customers in the same way, the business can use different marketing strategies for different customer groups based on their purchasing behaviour.

## Files

- `level01task02customersegmentation.ipynb` – Jupyter Notebook containing the complete analysis
- `customer_dataset.xlsx` – Dataset used for the project
