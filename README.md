# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the necessary packages using import statement.

2.Read the given csv file using read_csv() method and print the number of contents to be displayed using df.head().

3.Import KMeans and use for loop to cluster the data.

4.Predict the cluster and plot data graphs.

5.Print the outputs and end the program

## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: LATHIKA L J
RegisterNumber:  212223220050

import pandas as pd
import matplotlib.pyplot as plt
data=pd.read_csv('Mall_customers.csv')
data.head()

data.info()

data.isnull()

data.isnull().sum()

from sklearn.cluster import KMeans
wcss=[]

for i in range(1,11):
    kmeans=KMeans(n_clusters =i,init ="k-means++")
    kmeans.fit(data.iloc[:,3:])
    wcss.append(kmeans.inertia_)


plt.plot(range(1,11),wcss)
plt.xlabel("No. of Clusters")
plt.ylabel("wcss")
plt.title("Elbow Method")

km =KMeans(n_clusters=5)
km.fit(data.iloc[:,3:])

y_pred =km.predict(data.iloc[:,3:])
y_pred

df0.head()

df1.head()

df2.head()

df3.head()

df4.head()

plt.scatter(df0["Annual Income (k$)"],df0["Spending Score (1-100)"],c="red",label="cluster0")
plt.scatter(df1["Annual Income (k$)"],df1["Spending Score (1-100)"],c="blue",label="cluster1")
plt.scatter(df2["Annual Income (k$)"],df2["Spending Score (1-100)"],c="green",label="cluster2")
plt.scatter(df3["Annual Income (k$)"],df3["Spending Score (1-100)"],c="black",label="cluster3")
plt.scatter(df4["Annual Income (k$)"],df4["Spending Score (1-100)"],c="magenta",label="cluster4")
plt.legend()
plt.title("Customer Segments")
*/
```

## Output:
![image](https://github.com/user-attachments/assets/926eb58d-bee9-445e-8d30-0e6f41397537)
![image](https://github.com/user-attachments/assets/3e2bbe22-edaf-48c0-b037-1b7b4cc3e4b6)
![image](https://github.com/user-attachments/assets/b4df634a-0bc6-4cd2-9a06-3f3a59f4e051)
![image](https://github.com/user-attachments/assets/d434938b-e8a2-43ad-82a4-3a2dc1ea0e1e)
![image](https://github.com/user-attachments/assets/ff9f0066-ba60-4fae-a683-6403d787189c)

## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
