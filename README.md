# Data-Visualization-Challenge
Week 5-Challenge

**Background**
You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specialises in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumours received treatment with a range of drug regimens. Over the course of 45 days, tumour development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.

**Instructions**
Prepare the data.
Generate summary statistics.
Create bar charts and pie charts.
Calculate quartiles, find outliers, and create a box plot.
Create a line plot and a scatter plot.
Calculate correlation and regression.
Submit your final analysis.

**Task requirements**
1. Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.

2. Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.

3. Display the updated number of unique mice IDs.

**Generate Summary Statistics**
1. Create a DataFrame of summary statistics. 

2. Your summary statistics should include:

3. A row for each drug regimen. These regimen names should be contained in the index column.

4. A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumour volume.

**Create Bar Charts and Pie Charts**
1. Generate two bar charts. Both charts should be identical and show the total number of time points for all mice tested for each drug regimen throughout the study.

2. Create the first bar chart with the Pandas DataFrame.plot() method.

3. Create the second bar chart with Matplotlib's pyplot methods.

4. Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

5. Create the first pie chart with the Pandas DataFrame.plot() method.

6. Create the second pie chart with Matplotlib's pyplot methods.

**Calculate Quartiles, Find Outliers, and Create a Box Plot**
1. Calculate the final tumour volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. 2. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. 

Use the following substeps:

1） Create a grouped DataFrame that shows the last (greatest) time point for each mouse (Using Max function). Merge this grouped DataFrame with the original cleaned DataFrame.

2） Create a list that holds the treatment names as well as a second, empty list to hold the tumour volume data.

3） Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumour volumes for each drug to the empty list.

4） Determine outliers by using the upper and lower bounds, and then print the results.

Using Matplotlib, generate a box plot that shows the distribution of the final tumour volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.

Hint: All four box plots should be within the same figure. Use this Matplotlib documentation pageLinks to an external site. for help with changing the style of the outliers.

**Create a Line Plot and a Scatter Plot**
1. Select a mouse that was treated with Capomulin, and generate a line plot of tumour volume versus time point for that mouse.

2. Generate a scatter plot of tumour volume versus mouse weight for the Capomulin treatment regimen.

**Calculate Correlation and Regression**
1. Calculate the correlation coefficient and linear regression model between mouse weight and average tumour volume for the Capomulin treatment.

2. Plot the linear regression model on top of the previous scatter plot.
-----End-------
