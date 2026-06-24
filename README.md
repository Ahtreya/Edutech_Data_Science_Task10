# Edutech_Data_Science_Task10
## Task 10: Customer Segmentation using K-Means Clustering

### 📌 Project Overview
This project applies Unsupervised Machine Learning (K-Means Clustering) to segment mall customers based on their demographic and behavioural data using Scikit-Learn.

### 🛠️ Steps Performed
1. **Data Cleaning:** Removed irrelevant columns (`CustomerID`) to maintain clean feature matrices.
2. **Label Encoding:** Converted categorical column (`Genre`) into standardised numerical levels.
3. **Feature Scaling:** Applied `StandardScaler` to ensure distance matrices are not distorted by differing numeric scales.
4. **Elbow Method:** Calculated and plotted Within-Cluster Sum of Squares (WCSS) to identify the optimal cluster change inflexion point ($K=4$).
5. **Model Evaluation:** Assigned cluster index tags using the `fit_predict` workflow.

### ❓ Interview Questions Answered
* **How do you choose 'K'?**  
  We use the **Elbow Method** by plotting the WCSS (Within-Cluster Sum of Squares) values against a range of cluster quantities. The exact point where the sharp reduction in error slows down and forms a distinct "elbow" or bend, marks our optimal $K$ choice (which is $K=4$ for our combined scaled features).
* **What are centroids?**  
  Centroids represent the **geometric mean centre points** of each cluster. Every customer point inside a specific cluster is matched to its nearest centroid based on the minimised spatial Euclidean distance.
