# wine-quality-prediction
Regression and classification model  for wine quality prdiction


This README file contains requirements and environment to run the winequality model notebook.
1.	The data was downloaded from http://archive.ics.uci.edu/ml/datasets/Wine+Quality, and saved as winequality-red.csv and winequality-white.csv. They are formatted  csv files.
2.	Winequality.names is downloaded from the website and it describes the dataset. Based on its description, we know that the data is clean, with no missing values, and it’s not balanced. The correlation among the variables are not studied. It does mention that for high and low quality wines, there are much fewer data to be able to provide for the model building
3.	Wineqamodel.ipynb is the jupyter notebook developed to build the model.  The environment is Anaconda 3(64bits) for python 3.6.
4.	The notebook is self-explanatory on the step-by-step model building, please read the comments carefully on each step.
5.	The code and dataset are in the same directory, and it is assumed the working directory of jupyter notebook is the same. Otherwies, please change the directory accordingly as shown in step 1 to be able to access the dataset.
6.	Libraries or packages are used in the code, so please make sure the same ones are installed to run the code: pandas, numpy, matplotlib, seaborn, sklearn, statsmodels.
7.	A html file is generated from the ipynb file, and it’s named winequalitymodelbuilding.html. You can understand the steps without running the code. 
8.	The notebook contains the explanation on the model selection and evaluation.
9.	One column or variable was dropped after it’s found that it’s highly correlated with another variable
10.	The data is highly imbalanced, so oversampling is needed, but skipped here
11.	Two methods were studied: regression and classification. For regression, multilinear and random forest are used, and for classification, random forest was used.
12.	The boosting method could be used to improve the result, because the some classes(high and low) have only a few instances, e.g., Adaboost, gradient boosting, XGboost. But it’s skipped here.
13.	The model can provide reasonable prediction on normal classes of wines, but it is misleading for high end and low quality wines, the results cannot be trusted for these classes.
14.	The model can be improved with more data and better data, especially for high and low end wines.
