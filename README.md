
# MLS-Project
Machine Learning &amp; Statistics Project for 2019

## Assignment Instructions
Using one Jupyter notebook;
1. Conduct an analysis of the Boston House Price data using descriptive statistics & plots. (20%).
2. Use inferential statistics to analyse if there is a significant difference between the median house prices between those along the charles river and those that are not. (20%).
3. Create a neural network that can predict the median house price based on the other variables. (60%).

## Initial Approach
1. Research to see what is written about the Boston House Prices dataset.
2. Gather credible external sources for reference and write a small literature review.
3. Conduct my own analysis of the Boston House Prices dataset.
4. Using ANOVA determine if there is a significant difference in median house prices between properties along the Charles river and those that are located elsewhere.
5. Utilise external sources to help the discussion.
6. Create initial neural network to predict the median house price based on the other varibales.
7. Compare the predictions to the expected values in the original dataset.
8. Utilse my own analysis of the Boston House Prices dataset to train and tune the neural network.
9. Compare the enhanced predictions to the expected values in the original dataset.
10. Draw balanced conclusions.

## Method
Looking at scikit learn library
from sklearn.datasets import load_boston //use scikit-learn to import dataset - I have csv
boston_dataset = load_boston() //name it
print(boston_dataset.keys()) // print Desc like in MySQL 
dict_keys(['data', 'target', 'feature_names', 'DESCR']) //result
boston_dataset.DESCR //just look at descriptions

target variable is MEDV // median value
feature variables used to predict target variables // 

boston = pd.DataFrame(boston_dataset.data, columns=boston_dataset.feature_names) //pandas DF
boston.head()

## Research
In order to get an idea of what the dataset is about it is best to start with what has been previously said about the dataset and from there we can look at a number of concepts.

### Basic Analysis
The simplest way to get started is by looking at the dataset firstly through some descriptive statistics
https://subscription.packtpub.com/book/programming/9781789804744/1/ch01lvl1sec11/our-first-analysis-the-boston-housing-dataset

### Feature observation
Trying to interpret which features are powerful indicators and useful later and which have less of a correlation to the median house prices in Boston.
https://www.ritchieng.com/machine-learning-project-boston-home-prices/

### Linear regression
The clearest way to look at the dataset in relation to the target variable MEDV is to look for positively and negatively correlated feature variables
https://towardsdatascience.com/linear-regression-on-boston-housing-dataset-f409b7e4a155 

### Other ideas

https://levelup.gitconnected.com/predict-boston-house-prices-using-python-linear-regression-90469e0a341

https://gogul.dev/software/regression-example-boston-housing-prices

#### Original ideas
https://www.ritchieng.com/machine-learning-project-boston-home-prices/

https://medium.com/@haydar_ai/learning-data-science-day-9-linear-regression-on-boston-housing-dataset-cd62a80775ef

http://www.neural.cz/dataset-exploration-boston-house-pricing.html

https://www.kaggle.com/erick5/predicting-house-prices-with-machine-learning

https://rstudio-pubs-static.s3.amazonaws.com/364346_811c9012a14847428c9b1fc1e956431a.html

https://www.kaggle.com/sagarnildass/predicting-boston-house-prices

https://www.hackerearth.com/practice/machine-learning/machine-learning-projects/python-project/tutorial/


#### Designing & Tuning Neural Network
https://towardsdatascience.com/a-guide-to-an-efficient-way-to-build-neural-network-architectures-part-i-hyper-parameter-8129009f131b