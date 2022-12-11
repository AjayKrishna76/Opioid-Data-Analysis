# Opioid-Data-Analysis
## U.S. Opioid Epidemic Analysis

This is a repository where the analysis for the Opioid Epidemic in United States is performed.

Main aim is to collect the data from different datasets such as Drug Overdose Dataset, County Health Rankings, County Opioid Dispensing Rates and understand and visualize them with the help of Data Science techniques to estimate the impact of Opioid Epidemic across different socio-economic, demographic, geographic variables that are present for the counties in US and to give future predictions.

![opioid](https://www.hhs.gov/opioids/sites/default/files/inline-images/opioids-infographic.png)

## Structure of this repository
***
|-- README.md                       # the README file of this repo 📖 

|-- data                            # the datasets used in this repository 📃

|-- docs                            # documentation of the project reports and presentations📗

|-- images                          # All the images/plots/graphs generated are found here 📉📈

|-- src                             # the code and notebooks! 📚📚

|-- utilities                       # scripts used for the data 📃

|-- requirements                    # Packages required/used in this project


## Software used (open source):
***
+ [python](https://www.python.org/download/releases/3.0/)
+ [NumPy](https://numpy.org/)
+ [pandas](https://pandas.pydata.org/)
+ [plotly](https://plotly.com/)
+ [Jupyter Notebook](https://jupyter.org/)
+ [Seaborn](https://seaborn.pydata.org/)
+ [Scipy](https://scipy.org/)



## Stage I - Data Understanding and Linking.
***
In this stage different datasets are aquired. The below links can be used to download these datasets.

+ [Drug Overdose Dataset](https://wonder.cdc.gov/ucd-icd10.html)
+ [County Health Rankings](https://www.countyhealthrankings.org/)
+ [County Opioid Dispensing Rates](https://www.cdc.gov/drugoverdose/maps/rxcounty2019.html)

#### Opioid overdose dataset linking - tasks performed:
- In stage 1, different datasets available are linked to obtain a super dataframe which can be used for further analysis.
- Analyse the different variables present in the data and formulate a data dictionary.
- Identifying issues with the data.
- Identifying the top counties and states with highest opioid mortality rates.

## Stage II - Data Modeling.
***
In this stage the data for modelling and comparitive analysis is developed. Here I am analysing county based information for different states in the US.
- Dataset used in this stage is [opioid  related mortality from 1999-2019](https://wonder.cdc.gov/wonder/help/ucd.html#Drug/Alcohol%20Induced%20Causes)

#### Tasks Performed:
- In this stage we are graphically comparing how different states are doing with respect to opioid mortality rate.
- Histogram plot with mean and median of Normalized Deaths for entire US as a distribution.
- Adding a label column by performing a quantile distribution of the Normalized Deaths.
- Plotting the variables identified in stage1 (Scatter Plot). Developing an interactive method to display all the variables in Plotly widget for jupyter.[Plotly Widget](https://plotly.com/python/figurewidget-app/)
- Calculating the mean opioid mortality for states and US per year. Identifying the peaks in the data.
- Identifying the relation between mortality and population of a state.


## Stage III - Distributions and Hypothesis Testing.
***
#### Task1: Distribution Analysis:
- Analysing the distribution of the data with respect to different states in the US.
- Developing the distribution estimators with Method Of Moments (MOM), Most Likelihood Estimate (MLE) and Kernel Density Estimator (KDE).
#### Task2: Hypothesis Testing and Regression:
- In this task we are performing hypothesis testing on the data. Selecting 5 different variables in the data to perform hypothesis testing, on analysis different testing methods a Two sample T-Test is performed by formulating a Null Hypothesis.
- With the help of this test we can come to a conclusion on the different variables which have an impact on the opioid deaths with respect to state level.
- For regression, different forms of regression are considered. A simple linear regression was performed on the data with respect to opioid martality rate to look at the trend in the data. A multiple linear regression was performed on the data containing five different variables as a single entity with respect to opioid mortality rate. Polynomial Regression was performed for the data and a best fir curve is estimated. All the model performance scores were extracted to compare different regression models on the data. A multinodal higher order regression was performed as well. 

## Stage IV - Dashboard.
***
Developing a simple interactive dashboard. Utilizing [plotly](https://plotly.com/) along with the [Dash](https://plotly.com/dash/) as a framework.
- All the above performed tasks were shown in a single dashboard. Here the data is presented visually in the United States map and the data table is also shown which contains the data on the specific selection with respect to different state level data as well as the whole data of US.

![Dashboard](https://github.com/AjayKrishna76/Opioid-Data-Analysis/blob/main/images/ajay/stage_4/2.png)

### Project Setup:
***
1. Clone the repository - Clone the repository by pasting this [link](https://github.com/AjayKrishna76/Opioid-Data-Analysis) in your favorite terminal.
2. Make sure you have the above used Software in your local machine.
3. Some additional python packages required to run the code properly can be installed by running the following code.

```
pip install -r requirements.txt
```
