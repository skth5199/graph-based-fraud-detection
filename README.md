# Fraud Detection using Graph Machine learning
This repository consists of a solution that includes the analysis of financial data and detection of Fraud detection using Graph Machine Learning. The solution uses a Relational Graph Convolutional Network that generates unique graph features from neighbourhood information to aid in better and effective detection of fraud.

The setps are as follows:
1. Pre-processing
2. Making edgelists using the user identity columns
3. Generating a multi dimensional heterogenous graph using the data along with these edgelists 
4. Using the Deep Learning models to generate predictions

The dataset used was the IEEE-CIS Fraud Detection Dataset provided by [Vesta](https://www.vesta.io/) on [Kaggle](https://www.kaggle.com/c/ieee-fraud-detection)

Two RGCN (Relational Graph Convolutional Networks) were developed and tested
1. Shallow RGCN
2. Deep RGCN

Despite the heavy class imbalance, the Deep RGCN produced great results and outperformed the shallow RGCN. The evaluation metric scores were as follows:
* F1: 0.6228 (Shallow network 0.48)
* Accuracy: 98% (Shallow network 97.48%)
* Precision: 0.8872 (Shallow network 0.8240)
* Recall: 0.4798 (Shallow network 0.3410)
* Confusion matrix:


|          | Predicte Positive | Predicted Negative |
| -------- |:-----------------:| ------------------:|
| Positive |              1950 |                248 |
| Negative |              2114 |             113796 |

The architecture of the solution is as follows:
<p align="center">
<img src=https://user-images.githubusercontent.com/26760537/164785640-9f4aa117-dcd5-4aeb-b4bc-77e1ac65b05c.png>
</p>

To run the code, simply run the Jupyter notebooks in this order:
1. DataPrep
2. Modelling
3. Visualization
