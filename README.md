# All Life Bank Customer Segmentation for Credit Card Services

## Context
AllLife Bank (ALB) wants to focus on its credit card customer base in the next financial year. ALB has been advised by its marketing research team (MRT), that the market penetration can be improved. Based on this premise, the Marketing team proposes to run personalized campaigns to target new customers as well as upsell to existing customers. Another insight from the MRT was that customers perceive the support services of ALB poorly. Considering these, the Operations team wants to improve the service delivery model to ensure that customer queries are resolved faster. The head of Marketing and the head of Delivery decide to reach out to the Data Science team for help.

![](https://i.imgur.com/1XPO1qk.jpg)

## Problem Definition
Credit Card services present these problems:

- Market Penetration has to increase.
- Current Customer's Credit Card Services should increase.
- Credit Card Customer Support is perceived as poor.
- Credit Card Customer's Queries should be resolved faster.

Identify (classify) the different segments in the existing customer base, based on their spending patterns, past interaction with the bank, and any other important data available.
Specify the characteristics of each segment and notice the weak or strong patterns of each segment.
Provide recommendations to ALB for each segment based on items 1 and 2 above. These recommendations should include how to expand the market penetration (new and current customers) and how to improve the customer services. Possibly recommend what type of service feature is important for each segment.

**Data Dictionary**

The data provided is of various customers of ALB and their financial attributes like credit limit, the total number of credit cards the customer has, and different channels through which customers have contacted the bank for any queries (including visiting the bank, online and through a call center).

- Sl_No: Primary key of the records
- Customer Key: Customer identification number
- Average Credit Limit: Average credit limit of each customer for all credit cards
- Total credit cards: Total number of credit cards possessed by the customer
- Total visits bank: Total number of visits that the customer made (yearly) personally to the bank
- Total visits online: Total number of visits or online logins made by the customer (yearly)

- Total calls made: Total number of calls made by the customer to the bank or its customer service department (yearly)

## **Questions**

Formulating Questions after knowing what type of data is available helps us formulate better questions.

Q1. How can the customers be grouped/segmented (classified)?
Q2. What are the commonalities of each group/segment? ie:
- Total/Particular Interaction w/ ALB
- Total Credit Cards
- Average Credit Limit
Q3. What is the group/segment that has the most/least interactions/particular type of interaction with ALB?
Q4. Is there a relationship between Average Credit Limit/Total Credit Cards and customer satisfaction (assuming that the number of interactions is an indication of unsolved issues)?
Q5. What is the relationship between Average Credit Limit/Total Credit Cards to interactions/type of interactions with ALB (this question is partially addressed by Q2)?
Q6. What recommendations can be made for each group/segment to improve customer satisfaction (assuming that the number of interactions is an indication of unsolved issues)?
Q7. What recommendations can be made based in segment characteristics to increase market penetration/expand services to current customers?
With this set of questions, we address the problems introduced earlier and make recommendations to ALB.

## Technique
This is an unsupervised classification problem. We will classify customers into different segments using K-means Clustering and Hierarchical Clustering algorithms.
Perform the data preprocessing, EDA analysis, and feature engineering. We will visualize features and observe relationships performing a uni and bivariate analysis.
Attempt the classification using the K-means clustering. We will estimate the better number of clusters using the elbow method and observe silhouettes. Then we will visualize the clusters.
Attempt the classification using hierarchical clustering. We will explore clustering with different linkage methods (i.e. single, complete, etc) and distances (i.e. euclidean, manhattan, etc) reviewing the cophenetic correlation and find the ideal number of clusters. Then we will visualize the clusters.

Compare K-means vs Hierachical clustering results.
