# Technology Trends Analysis
## A project to analyze technology trends using data obtained from APIs, Web Scraping and Survey data
![](IMAGES/toptrendsjpg.jpg)
## Introduction
In order to keep pace with changing technologies and remain competitive, organizations regularly analyze data to help identify current technologies as well as future skill requirements.
This project aim is therefore to carry out technology trend analysis which will start with collecting data from various sources and  clean it up to make it suitable for the analysis.

##  Problem statement 
__what are the skill requirements for future?__
__What are the top programming languages in demand?__
__What are the top database skills in demand?__
![image](https://github.com/gessa2020/Technology_trends/assets/52911013/4dcc9eea-baf2-4980-b2a7-c1344de8e672)

 
 
<h4>Workflow</h4>
From the historical data, we will first train a machine learning clustering  model on customer profile variables to come up with target groups also known as clusters, there after, we will then train a classification model that can predict which cluster a customer belongs to so as to tailor specific products to the client depending on the charactistics of the cluster.

## Skills demonstrated.
- Python was used for coding the project together with some data science algorithms as seen in the notebook
- I used jupyter notebooks as the main IDE for coding
- I used Visual Studio code to develop and deploy the streamlit application

## Data sourcing
I just wanted to get my hands dirty with customer segmentation, so i went to kaggle.com and and got my hands on to this  <a href="https://www.kaggle.com/datasets/sidharth178/customer-segmentation">Dataset</a> so as to practice my skills. 
 The sample Dataset summarizes the usage behavior of about nearly 1000 active credit card holders during the last 6 months. The file is at a customer level with 10 behavioral variables.
 These include:'Customer Id', 'Age', 'Edu', 'Years Employed', 'Income', 'Card Debt','Other Debt', 'Defaulted', 'DebtIncomeRatio'

## Data transformation and cleaning.
1.  I had to first drop the 'unnamed 0' column since it was not meaningful for our project.
3.  There was some missing data in the defaulted variable, so i filled it in with the median for that column.

## Data analysis and visualization
Graph showing distribution of individual numerical variables![](IMAGES/Histogram_image1.png)
### key take ways from the plot above
- The average age of clients is about 35 years with the age distribution being fairly skewed to the right
- Income and Card Debt are highly skewed to the right
- Debt income ratio and years employed have distributions that are skewed to the right.
- The highest number of clients have education in category 1.0

Graph showing Generated Clusters![](IMAGES/cluster_image.png)
## Cluster building
To perform clustering, we had to preprocess the data using principle component analysis algorithm to produce two principle componets as our dimensions to be used in the clustering process.These were used to generate the clusters as seen in the image above. Further anlysis was performed to find the ideal number of clusters to be used in our data.We considered the ideal number of clusters to be used as 3 that can be seen in the graph above.

Graph showing cluster analysis with data![](IMAGES/clusterstat.jpg)
Having performed some statistics on the generated clusters, we can draw the following conclusions
1. Cluster 1 has the highest average income of about 13k and average age of 46 years.This can be considerd as a high value target cluster for banking products such as loans and savings.
2. Cluster 2 has the least average income of about 9.4k and has the least average age of 29 years. This can be a target cluster for bank products such as mortgage and credit card
3. Cluster 0 has a moderate average income of about 9.7k and has the higest average age of 84 years. This can be a target cluster for bank products such as pension


## Final model buiding and evaluation
Model performance graph![](IMAGES/modal_image1.png)

A range of models were trained on the data and their performance assessed as seen in the bar graph above.
The gradient boosting classifier and the Random forest model were the best performing classifers.
Further analysis was performed to know which of them was the better model.The Random forest emerged as the slightly better model by comparing the performance of thier classification reports and confusion matrices. 
The best performing model was saved for use in the streamlit application.

## Model deployment
Streamlit Application user interface![](IMAGES/streamlitapp.jpg)

## Conclussion

1. The clusters generated give us some useful information about our customer base such as their average income,
   age,debt to income ratio, education and years employed. 
2. We can use the statistics about these clusters to know where each customer belongs to.
3. With this information, we can then be able to tailor our bank products such as savings, loans, mortgage
   credit card to specific customers depending on the cluster they belong to for better performance of marketing     campaigns.

