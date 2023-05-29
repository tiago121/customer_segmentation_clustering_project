# e-commerce_customer_segmentation-


#### Made by Tiago Araujo

# Description

Customer segmentation project, using clustering algorithms, for a marketplace.

# 1. Business Problem

An online marketplace with a variety of products struggles to understand its customers and believes that the best strategy to reduce costs is to maximize customer retention. 
To achieve this, they need a model that automatically identifies customer profiles and groups. 
The results will be passed on to the marketing team to develop new retention strategies.

# 2. Solution Strategy

**Step 01: Data Description and Cleaning**

The data is from the Kaggle platform and consists of information about customer transactions: https://www.kaggle.com/code/fabiendaniel/customer-segmentation/data

* Objective: Understand and organize the data for manipulation and analysis.
* Process: Rename and adjust variable types; describe numerical/categorical variables; fill in missing data.

**Step 02: Data Filtering**

* Objective: Select the appropriate data subset for analysis.
* Process: Filter based on "unit_price" and "quantity" variables; remove outliers.


**Step 03: Feature Engineering**

* Objective: Facilitate analysis and discover new insights.
* Process: Create a new dataset with unique customers to aggregate customer information. 


**Step 04: Exploratory Analysis**

* Objective: Gain intuitive understanding of the data and how it varies over time.
* Process: Plot variable distributions.


**Step 05: Data Preparation and Dimensionality Reduction**

* Objective: Prepare the data for model training.
* Process: Rescale and reduce dimensionality.


**Step 06: Algorithm Selection**

* Objective: Select the best algorithms that combine dimensionality reduction and clustering.
* Process: Train and evaluate algorithms; compare different silhouette coefficients.


**Step 07: Training the Final Model**

* Objective: Train the best model.
* Process: Use UMAP (dimensionality reduction) and K-means (clustering) algorithms.


**Step 08: Cluster Analysis**

* Objective: Understand the characteristics of each cluster and translate them into valuable business insights.
* Process: Create a table with aggregated cluster information using groupby.


# 3. Model Evaluation

To evaluate the models, the silhouette coefficient metric was used. It measures the quality of clustering, with higher values indicating well-defined and separated clusters. A score close to 1 suggests distinct clusters, while a score around 0 implies overlapping clusters. Negative values indicate incorrect cluster assignments. which calculates intra-cluster and inter-cluster distances, indicating how well the clusters are formed, ranging from -1 to 1.

![image](https://user-images.githubusercontent.com/88745881/207449729-6bd184c4-9d64-4dbb-b1d7-26520115bbb5.png)


# 4. Business Results

The best-performing model, considering the business strategy, created 8 different groups:


**Cluster 1:**

* Number of customers: 9% of customers
* Average Recency: 288 days
* Average Products Purchased: 460 products
* Average Product Frequency: 0.76 products/day
* Average Revenue: $242.00 USD
* Strategy: Send discount coupons more frequently to encourage loyalty and reduce recency

**Cluster 2:**

* Number of customers: 9% of customers
* Average Recency: 38 days
* Average Products Purchased: 1102 products
* Average Product Frequency: 0.03 products/day
* Average Revenue: $323.00 USD
* Strategy: Since this group makes large purchases, show ads for similar products to encourage more diverse purchases.

**Cluster 3:**
* Number of customers: 13% of customers
* Average Recency: 21 days
* Average Products Purchased: 506 products
* Average Product Frequency: 0.76 products/day
* Average Revenue: $389.00 USD
* Strategy: Due to resource constraints, do not engage with this group at the moment and monitor their behavior.

**Cluster 4:**
* Number of customers: 12% of customers
* Average Recency: 53 days
* Average Products Purchased: 254 products
* Average Product Frequency: 1 product/day
* Average Revenue: $341.00 USD
* Strategy: Send discount coupons more frequently to encourage loyalty and reduce recency.

**Cluster 5:**
* Number of customers: 12% of customers
* Average Recency: 74 days
* Average Products Purchased: 501 products
* Average Product Frequency: 0.5 products/day
* Average Revenue: $139.00 USD

**Cluster 6:**

* Number of customers: 6% of customers
* Average Recency: 285 days
* Average Products Purchased: 389 products
* Average Product Frequency: 0.8 products per day
* Average Revenue: $405.00 USD
* Strategy: Send discount coupons more frequently to encourage loyalty and reduce recency.

**Cluster 7:**

* Number of customers: 23% of customers
* Average Recency: 11 days
* Average Products Purchased: 2575 products
* Average Product Frequency: 0.04 products per day
* Average Revenue: $583.00 USD
* Strategy: Establish a specialized customer service channel for this group to encourage continued purchasing behavior.

**Cluster8:**

* Number of customers: 14% of customers
* Average Recency: 235 days
* Average Products Purchased: 230 products
* Average Product Frequency: 0.9 products per day
* Average Revenue: $248.00 USD
* Strategy: Send emails with cheaper products to stimulate more frequent purchases.

# 5. Conclusion

* By implementing customer segmentation through clustering, the business can effectively focus its marketing strategies and tailor offers to specific customer groups
* Automating the clustering process ensures continuous relevance and accuracy as new customers enter and existing ones change their profiles.

# 6. Next Steps


The following steps are recommended for further development and improvement of the project:

* Test alternative algorithms for dimensionality reduction and clustering to explore potential enhancements and optimize results.
* Transition the developed model into production to enable real-time customer segmentation and support ongoing marketing efforts. This involves integrating the model into the existing system infrastructure and ensuring its seamless operation and scalability.








