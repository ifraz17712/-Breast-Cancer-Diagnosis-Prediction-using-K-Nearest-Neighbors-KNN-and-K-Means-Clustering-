# -Breast-Cancer-Diagnosis-Prediction-using-K-Nearest-Neighbors-KNN-and-K-Means-Clustering-
Here is the same information rewritten with a different tone and phrasing, as if written by another person:

---

**Problem Overview:**
This project focuses on classifying breast cancer cases using two machine-learning techniques: K-Nearest Neighbors (KNN) for supervised classification and K-Means clustering for unsupervised grouping.

**Data Preprocessing Steps:**

* **Encoding the Diagnosis:**
  To make the target variable compatible with the models, the diagnosis column was converted into numeric values—malignant cases were assigned a value of 1, while benign cases were labeled as 0.

* **Removing Unnecessary Columns:**
  The *id* column was dropped since it doesn’t add any predictive value. Another column, *Unnamed: 32*, contained only missing values, so it was removed to keep the dataset clean.

* **Handling Missing Data:**
  After removing irrelevant columns, the dataset was checked for missing entries. Any rows or columns containing null values were removed to preserve the reliability of the dataset.

* **Applying Min-Max Normalization:**
  All feature columns (except the diagnosis label) were scaled to a range between 0 and 1. This step is crucial because both KNN and K-Means rely heavily on distance calculations, and unscaled features could distort their performance.

* **Splitting the Data:**
  The dataset was divided into an 80% training set and a 20% testing set. The training set was used to train the models, while the test set allowed for an objective evaluation of their performance.

**Algorithms Applied:**

* **K-Nearest Neighbors (KNN):**
  A supervised learning algorithm that predicts the class of a sample by examining the most common class among its closest neighbors.

* **K-Means Clustering:**
  An unsupervised algorithm that partitions the data into two clusters, helping reveal natural groupings between benign and malignant cases.

**Model Performance:**
The KNN classifier achieved strong results on the test set, with the following metrics:

* **Accuracy:** 0.9649
* **Precision:** 0.9535
* **Recall:** 0.9535
* **F1-Score:** 0.9535

These metrics reflect a well-performing and balanced model. Additionally, K-Means clustering showed clear separation between the two types of cases, indicating that the dataset has a naturally distinguishable structure.


