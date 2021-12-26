# ENSF-612_Project

An extension to the paper ColBERT: Using BERT Sentence Embedding for Humor Detection by Issa Annamoradnejad, Gohar Zoghi (https://arxiv.org/abs/2004.12765), this project 
(1) Verifies the difference in accuracy between the ColBERT Sentence Embedding model versus baseline models and
(2) Determines if the baseline model can also distinguish between satire and non-satire humour.

In order to achieve objective (1), the baseline models are replicated and the hyperparameters are tuned in order to achieve the highest possible accuracy for a baseline model. This is used to compare to the accuracy of the ColBERT Sentence Embedder model. In order to achieve objective (2), 1000 additional data points of satirical and non-satirical humour are added to the dataset. This allows us to test the accuracy on the original + new dataset.

### Results
Logistic Regression ML model with 0.1 (regularization hyperparameter) performed at an F1-Score of 93.2%. Multinomial Naive Bayes with a 0 (smoothing parameter) performed at an F1-Score of 93.1%. Both results are using the combined datasets (including satire data points).

### Conclusion
Overall, we were able to (1) extend the baseline model from the original paper to satire vs non-satire, and (2) verify that the 93.2% F1-Score achieved by the baseline models is still 6% less than the 98.2% F1-Score achieved by the ColBERT model.

How to open notebook:
1) Create Databricks Community Edition (Free) Account
2) Import Group11-ProjectCode.ipynb into workspace
