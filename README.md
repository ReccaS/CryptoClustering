# Cryptocurrency Market Data Analysis

This project analyzes cryptocurrency market data using KMeans clustering and Principal Component Analysis (PCA). The code performs data preprocessing, clustering, and visualization to group cryptocurrencies based on their market performance over different time periods.

## **Table of Contents**
* Installation
* Usage


## Installation

To run the code, you need to have the following Python libraries installed:
* pandas
* scikit-learn
* matplotlib


**You can install these libraries using !pip install**

**Import Required Libraries and dependencies**

![image](https://github.com/user-attachments/assets/e1bcc3f1-5800-46ae-9950-e1d4f0c9f0a1)

## Usage

1. **Load Data**

* Load the cryptocurrency market data from a CSV file into a Pandas DataFrame and set the index to coin_id.

![image](https://github.com/user-attachments/assets/9a991d6d-a7c6-4624-9629-f8a2ebf9fc2a)

2. **Data Preprocessing**

* Normalize the data using StandardScaler

![image](https://github.com/user-attachments/assets/5c15c508-ec4b-415c-b700-2bf33564538a)

3. **Elbow Curve to Determine Optimal k**

  * Compute the inertia for different values of k and plot the Elbow curve.

![image](https://github.com/user-attachments/assets/25bcdeb4-a936-45fb-85d4-bb7584e7059d)

![image](https://github.com/user-attachments/assets/26d9eecf-a548-488c-84d3-0bb2698cbbd2)


4. **KMeans Clustering**

* Cluster the cryptocurrencies using KMeans with the optimal value of k.

![image](https://github.com/user-attachments/assets/255869e8-adb5-42bd-881a-c81eaa66f8c3)

![image](https://github.com/user-attachments/assets/aa4e0483-3ef5-4db4-822b-29fa2aa3255d)

![image](https://github.com/user-attachments/assets/2c5dc5a3-f137-4166-a36d-614274bddedd)

5. **Principal Component Analysis (PCA)**

* Reduce the data to three principal components and analyze the variance.

![image](https://github.com/user-attachments/assets/d7320d06-a903-4324-be42-ac34420b4e9d)

6. **Elbow Curve with PCA Data**

* Determine the optimal k using the PCA data and plot the Elbow curve.

![image](https://github.com/user-attachments/assets/363a1691-860d-4c0c-bf94-be1ebd977fb8)

![image](https://github.com/user-attachments/assets/a9d65a49-ce38-4b17-98df-f8949d978286)


7. **Cluster Cryptocurrencies with PCA Data**

* Cluster the cryptocurrencies using the PCA data.

![image](https://github.com/user-attachments/assets/65ba7b77-9b1e-412f-8f62-5afda17df974)

![image](https://github.com/user-attachments/assets/960f2055-512a-440a-b5b6-eb8e238d54f2)

![image](https://github.com/user-attachments/assets/eb91b49c-a381-461c-a3b9-3eed005de8a1)


8. **Determine Feature Weights**

* Analyze the weights of each feature on each principal component.

![image](https://github.com/user-attachments/assets/6115d051-1877-45f6-a6b7-965fef38181c)

#### Answer the following question: 

* **Question:** Which features have the strongest positive or negative influence on each component? 
 
* **Answer:** 

PCA1

* Strongest Positive Influence: price_change_percentage_200d (0.594468)

* Strongest Negative Influence: price_change_percentage_24h (-0.416728)

PCA2

* Strongest Positive Influence: price_change_percentage_30d (0.562182)

* Strongest Negative Influence: price_change_percentage_1y (-0.150789)

PCA3

* Strongest Positive Influence: price_change_percentage_7d (0.787670)

* Strongest Negative Influence: price_change_percentage_60d (-0.361377)



























  

  


  
