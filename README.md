# Ex-09-Data-Visualization-

## AIM
To Perform Data Visualization on a complex dataset and save the data to a file. 

# Explanation
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Clean the Data Set using Data Cleaning Process
### STEP 3
Apply Feature generation and selection techniques to all the features of the data set
### STEP 4
Apply data visualization techniques to identify the patterns of the data.


# CODE:
```python 
Developed by: harithashree.v
Register number:212222230046

import seaborn as sns
import matplotlib.pyplot as plt
tips=sns.load_dataset('tips')
tips

tips.head()

tips.info()

# Which day of the week has the highest total bill amount?

sns.barplot(x='day',y='total_bill',data=tips)
plt.title("Weekly highest total bill amount")

# What is the average tip amount given by smokers and non-smokers?

sns.barplot(x='smoker',y='tip',data=tips, palette='rainbow')
plt.title("Average tip amount given by smokers and non-smokers")

# How does the tip percentage vary based on the size of the dining party?

sns.boxplot(x='size', y='tip',data=tips)
plt.title("Tip percentage based on the sizes of the dining party")

# Which gender tends to leave higher tips?

sns.boxplot(x='sex', y='tip',data=tips)
plt.title("Higher tips based on gender")

# Is there any relationship between the total bill amount and the day of the week?

plt.plot(tips['day'],tips['total_bill'])
plt.title("Relationship between the total bill amount and the day of the week")
plt.show()

# How does the distribution of total bill amounts vary across different time periods (lunch vs. dinner)?

sns.violinplot(x='time',y='total_bill',data=tips)
plt.title("Distribution of total bill amounts vary across different time periods(lunch vs. dinner)")

# Which dining party size group tends to have the highest average total bill amount?

sns.barplot(x='size',y='total_bill',data=tips)
plt.title("Highest average total bill amount based party size")

# What is the distribution of tip amounts for each day of the week?

sns.boxplot(x='day',y='total_bill',data=tips)
plt.title("Distribution of tip amounts for each day of the week")

# How does the tip amount vary based on the type of service (lunch vs. dinner)?

sns.violinplot(x='time',y='tip',data=tips)
plt.title("Tip based on the type of service ")

# Is there any correlation between the total bill amount and the tip amount?

sns.scatterplot(data=tips, x='total_bill', y='tip')
correlation_coefficient = tips['total_bill'].corr(tips['tip'])
print("Correlation Coefficient:", correlation_coefficient)
# heatmap
tips.corr()
plt.subplots(figsize=(7,5))
sns.heatmap(tips.corr(),annot=True)
```

# OUPUT:
Ex-08-Data-Visualization-
AIM

To Perform Data Visualization on a complex dataset and save the data to a file.
Explanation

Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.
ALGORITHM
STEP 1

Read the given Data
STEP 2

Clean the Data Set using Data Cleaning Process
STEP 3

Apply Feature generation and selection techniques to all the features of the data set
STEP 4

Apply data visualization techniques to identify the patterns of the data.
CODE
Developed by: Sandhiya R
Register number:212222230129

import seaborn as sns
import matplotlib.pyplot as plt
tips=sns.load_dataset('tips')
tips

tips.head()

tips.info()

# Which day of the week has the highest total bill amount?

sns.barplot(x='day',y='total_bill',data=tips)
plt.title("Weekly highest total bill amount")

# What is the average tip amount given by smokers and non-smokers?

sns.barplot(x='smoker',y='tip',data=tips, palette='rainbow')
plt.title("Average tip amount given by smokers and non-smokers")

# How does the tip percentage vary based on the size of the dining party?

sns.boxplot(x='size', y='tip',data=tips)
plt.title("Tip percentage based on the sizes of the dining party")

# Which gender tends to leave higher tips?

sns.boxplot(x='sex', y='tip',data=tips)
plt.title("Higher tips based on gender")

# Is there any relationship between the total bill amount and the day of the week?

plt.plot(tips['day'],tips['total_bill'])
plt.title("Relationship between the total bill amount and the day of the week")
plt.show()

# How does the distribution of total bill amounts vary across different time periods (lunch vs. dinner)?

sns.violinplot(x='time',y='total_bill',data=tips)
plt.title("Distribution of total bill amounts vary across different time periods(lunch vs. dinner)")

# Which dining party size group tends to have the highest average total bill amount?

sns.barplot(x='size',y='total_bill',data=tips)
plt.title("Highest average total bill amount based party size")

# What is the distribution of tip amounts for each day of the week?

sns.boxplot(x='day',y='total_bill',data=tips)
plt.title("Distribution of tip amounts for each day of the week")

# How does the tip amount vary based on the type of service (lunch vs. dinner)?

sns.violinplot(x='time',y='tip',data=tips)
plt.title("Tip based on the type of service ")

# Is there any correlation between the total bill amount and the tip amount?

sns.scatterplot(data=tips, x='total_bill', y='tip')
correlation_coefficient = tips['total_bill'].corr(tips['tip'])
print("Correlation Coefficient:", correlation_coefficient)
# heatmap
tips.corr()
plt.subplots(figsize=(7,5))
sns.heatmap(tips.corr(),annot=True)

OUPUT
## dataset
![image](https://github.com/haritha-venkat/Ex-08-Data-Visualization_1/assets/121285701/2d207578-34b6-4780-911a-5f12f4c317a2)

## tips.head()
![image](https://github.com/haritha-venkat/Ex-08-Data-Visualization_1/assets/121285701/636b5ccb-0a51-410d-b077-355b988965b4)

## tips.info()
![image](https://github.com/haritha-venkat/Ex-08-Data-Visualization_1/assets/121285701/6269ed8a-612b-43cc-a35a-a5eecb2e281c)

![image](https://github.com/haritha-venkat/Ex-08-Data-Visualization_1/assets/121285701/962d6137-8977-4f6d-805a-16e6fe5a9e67)

![image](https://github.com/haritha-venkat/Ex-08-Data-Visualization_1/assets/121285701/ab31159e-33fd-4fa4-aba1-fefea43d29a8)

![image](https://github.com/haritha-venkat/Ex-08-Data-Visualization_1/assets/121285701/3c97a370-403b-48b2-92e0-4793b122f8de)

![image](https://github.com/haritha-venkat/Ex-08-Data-Visualization_1/assets/121285701/d70e9acf-699b-46ae-a96f-de730f23d8a4)

![image](https://github.com/haritha-venkat/Ex-08-Data-Visualization_1/assets/121285701/fb28bfda-d11a-4fd0-9655-334fb0879ded)

![image](https://github.com/haritha-venkat/Ex-08-Data-Visualization_1/assets/121285701/10ae1c3d-e8e3-4848-a83a-6ba833420358)

![image](https://github.com/haritha-venkat/Ex-08-Data-Visualization_1/assets/121285701/70a4e511-df87-4c3a-b08e-fac8c3cf6754)

![image](https://github.com/haritha-venkat/Ex-08-Data-Visualization_1/assets/121285701/e704da10-3894-4d50-81b1-f5171f9bfb35)

![image](https://github.com/haritha-venkat/Ex-08-Data-Visualization_1/assets/121285701/80f15242-436d-4a67-bb9c-21907b0388d0)

![image](https://github.com/haritha-venkat/Ex-08-Data-Visualization_1/assets/121285701/b48e3200-dfd6-48db-8d34-8df45af7f499)

![image](https://github.com/haritha-venkat/Ex-08-Data-Visualization_1/assets/121285701/a4fa45b7-3538-4a88-86ad-e175a04a907a)

## RESULT:

     Hence,Data Visualization is applied on the complex dataset using libraries like Seaborn and Matplotlib successfully based on tips dataset and the data is saved to file.
