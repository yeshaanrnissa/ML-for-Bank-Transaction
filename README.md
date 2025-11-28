# Machine Learning for Bank Transaction
This project analyzes bank transactions using machine learning methods with two main focuses:  
1. Clustering to find natural patterns in transactions and interpret the characteristics of each cluster.  
2. Classification by testing various algorithms, evaluating their performance, and performing hyperparameter tuning to find the best model.

## Dataset
The dataset can be downloaded here (direct download): https://drive.google.com/uc?id=1gnLO9qvEPqv1uBt1928AcsCmdvzqjC5m
The dataset contains bank transaction information such as transaction amount, transaction type, merchant/category, transaction time, and other supporting features.

## Project Objectives
1. Preprocess transaction data
2. Identify transaction patterns and groups using clustering and cluster interpretation
3. Try various classification models
4. Evaluate model performance
5. Perform hyperparameter tuning to find the best model
   
## Clustering Result
Based on the clustering analysis, the optimal number of clusters was K = 3. These three clusters were then further analyzed to understand the key characteristics of the customers within them.
1. Cluster 0 represents a group of customers with high transactions and high income, thus reflecting a segment of active users with strong purchasing power.
2. Cluster 1 consists of existing customers with low purchasing power, indicating the presence of a loyal user group but tending to have low transaction frequency or nominal value.
3. Cluster 2 contains regular customers with stable transaction activity, not particularly high but consistent over time.

Overall, the clustering model produced a Silhouette Score of 0.5403, indicating that the separation between clusters is quite good and the resulting cluster structure can be clearly interpreted.

## Classification Result
In the classification stage, several machine learning algorithms were tested to predict transaction categories. Each model was evaluated using four key metrics: Accuracy, Precision, Recall, and F1-Score. Overall, all models performed well, but several models stood out significantly.

The Decision Tree (DT) and Random Forest (RF) models performed best, with an accuracy of 0.9979, and consistently high precision, recall, and F1-scores around 0.998. This indicates that both models are capable of learning transaction patterns very well and have strong generalization capabilities to the test data.

The Support Vector Machine (SVM) model also performed very well, with an accuracy of 0.9792 and other evaluation metrics ranging from 0.978 to 0.979, making it a solid alternative, albeit slightly lower than RF and DT.

The Naive Bayes (NB) and K-Nearest Neighbors (KNN) models performed quite competitively, with accuracies of 0.9854 and 0.9417, respectively. Naive Bayes demonstrated stable performance across all metrics, while KNN had the lowest score among the tested models, although it still maintained a high level of accuracy.

Overall, Decision Tree and Random Forest performed best in this classification scenario, and therefore can be considered as the primary choices for the final model implementation.
