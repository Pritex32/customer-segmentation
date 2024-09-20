# customer-segmentation

## Table Of Content
-[Objective](Objective)

-[ Data Overview](data-overview)

-[Data Normalization](data-normalization)

-[Clustering with K-Means](clustering-with-k-means)

-[Cluster Analysis](cluster-analysis)

-[Visualization](visualization)

-[Recommendations](recommendations)


### Objective:
The goal of this project is  to develop customer segmentation to define a marketing strategy based on 
the behavior of around 9000 active credit card holders over the last six months.
The dataset contains 18 behavioral variables.

### Data Overview: (Download here)[https://www.linkedin.com/posts/prisca-ukanwa-800a1117a_see-how-you-can-increase-your-sales-with-activity-7241194742401667073-erx_?utm_source=share&utm_medium=member_desktop]
This  data includes variables such as CUST_ID, BALANCE, PURCHASES, CREDIT_LIMIT, and others related to credit card usage and payment behavior.
The dataset is imported using pandas, and
initial exploration which includes checking for missing values and duplicates. 
The dataset appears to have no missing values or duplicates after cleaning.

### Data Normalization:
Features are scaled using MinMaxScaler to normalize the data before clustering.

### Clustering with K-Means:
The elbow method is used to determine the optimal number of clusters, resulting in the choice of 4 clusters.
K-Means clustering is applied, and the data is segmented into four clusters.

### Cluster Analysis:
Each cluster is analyzed based on mean values of selected features:
- Cluster 0: High balance, infrequent purchases, and frequent advance payments. Contributes 7.4% to company sales.
- Cluster 1: Highest purchases, frequent transactions, main source of company sales, but no advance payments.
- Cluster 2: Moderate purchases, contributes 25.2% to sales, low credit limit, and no advance payments.
- Cluster 3: Lowest balance and purchases, infrequent transactions, 5.1% contribution to sales.

### Visualization:
Bar plots for average balance, payments, purchases, and cash advance per cluster are created using seaborn and matplotlib.
A pie chart shows the distribution of purchases across clusters.

### Recommendations:
- For Clusters 0 and 3: will encourage purchases through discounts, promotions, and personalized marketing communications.
- For Clusters 1 and 2: company should Increase thier credit limits and offer bonuses to stimulate more spending.
