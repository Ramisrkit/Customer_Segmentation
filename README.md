# Customer_Segmentation
# 👥 Customer Segmentation Using K-Means Clustering

## 🔍 Project Overview

This project focuses on **customer segmentation** using **unsupervised machine learning (clustering)** techniques. The goal is to group customers into meaningful segments based on their demographic and spending behavior, enabling businesses to design targeted marketing strategies.

The project uses the popular **Mall Customers dataset**, which contains information about customers such as age, income, and spending score.

---

## 🎯 Objective

* Identify distinct **customer groups** based on purchasing behavior
* Apply **K-Means clustering** to segment customers
* Determine the optimal number of clusters using evaluation techniques

---

## 📊 Dataset Description

The dataset consists of the following attributes:

| Feature                | Description                       |
| ---------------------- | --------------------------------- |
| CustomerID             | Unique customer identifier        |
| Gender                 | Customer gender                   |
| Age                    | Age of the customer               |
| Annual Income (k$)     | Annual income in thousand dollars |
| Spending Score (1–100) | Spending behavior score           |

> **Note:** There is **no target variable** in this dataset. It is an **unsupervised learning problem**.

---

## 🧠 Problem Type

* **Machine Learning Task:** Clustering (Unsupervised Learning)
* **Algorithm Used:** K-Means Clustering

This problem does not involve prediction or labels; instead, it focuses on discovering hidden patterns in customer behavior.

---

## ⚙️ Methodology

### 1️⃣ Data Preprocessing

* Removed unnecessary identifier column (`CustomerID`)
* Encoded categorical feature (`Gender`)
* Selected relevant numerical features:

  * Age
  * Annual Income (k$)
  * Spending Score (1–100)
* Applied **StandardScaler** to normalize features

---

### 2️⃣ Finding Optimal Number of Clusters

Two methods were used:

#### 🔹 Elbow Method

* Plotted **WCSS (Within-Cluster Sum of Squares)** vs. number of clusters
* Observed an elbow point at **k = 3**

#### 🔹 Silhouette Score

* Evaluated clustering quality for different values of k
* **k = 2** achieved the highest silhouette score (~0.45)

> Final selection considered both mathematical performance and business interpretability.

---

## ✅ Final Choice of k

* **Chosen k = 3**
* Reason: Balanced **cluster separation**, **interpretability**, and practical usefulness

---

## 🚀 Model Implementation

* Applied **K-Means clustering** with `k = 3`
* Assigned cluster labels to each customer
* Visualized clusters using scatter plots

---

## 📈 Evaluation

Since this is an unsupervised learning task:

* Accuracy is **not applicable** ❌
* Evaluation is done using:

  * Elbow Method
  * Silhouette Score
  * Visual inspection of clusters

---

## 🧩 Cluster Interpretation (Example)

| Cluster   | Description                                     |
| --------- | ----------------------------------------------- |
| Cluster 0 | Low income – Low spending                       |
| Cluster 1 | High income – High spending (Premium customers) |
| Cluster 2 | Medium income – Medium spending                 |

These segments can be used for **targeted marketing and customer engagement**.

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

---

## 📌 Conclusion

This project demonstrates how clustering techniques can be used to uncover meaningful customer segments without labeled data. By applying K-Means clustering and proper evaluation methods, the project provides actionable insights into customer behavior.

---

## 👤 Author

**Elliot**
Student | Machine Learning Enthusiast

---

⭐ If you find this project helpful, consider giving it a star!

