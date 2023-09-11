### Matplotlib Analysis
![module5pic1](https://github.com/kmorrow439/matplotlib_challenge/assets/114371722/e4618cad-5c2e-47a2-91c8-1f1110593cc0)
#### Background
##### You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.
##### As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.
##### The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.
---
##### Prepared the Data
##### 1.) Ran the provided package dependency and data imports, and then merged the "mouse_metadata" and "study_results" DataFrames into a single DataFrame.
##### 2.) Displayed the number of unique mice IDs in the data, and then checked for any mouse ID with duplicate time points. Displayed the data associated with that mouse ID, and then createed a new DataFrame where this data is removed. Used this cleaned DataFrame for the remaining steps.
##### 3.) Displayed the updated number of unique mice IDs.
---
#### Generated Summary Statistics
##### Created a DataFrame of summary statistics.
##### The summary statistics includes:
##### - A row for each drug regimen. These regimen names should be contained in the index column.
##### - A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.
---
#### Created Bar Charts and Pie Charts
##### 1.) Generated two bar charts. Both charts are identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.
##### - Created the first bar chart with the Pandas "DataFrame.plot()" method.
##### - Created the second bar chart with Matplotlib's "pyplot" methods.
![matplotlib7](https://github.com/kmorrow439/matplotlib_challenge/assets/114371722/264be94f-efe0-4905-95fb-5f1059a790bb)

##### 2.) Generated two pie charts. Both charts are identical and show the distribution of female versus male mice in the study.
##### - Created the first pie chart with the Pandas "DataFrame.plot()" method.
##### - Created the second pie chart with Matplotlib's "pyplot" methods.
![matplotlib2](https://github.com/kmorrow439/matplotlib_challenge/assets/114371722/317937b2-7a21-4db3-86f4-60dae308e269)
---
#### Calculated Quartiles, Find Outliers, and created a Box Plot
##### 1.) Calculated the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculated the quartiles and IQR, and determined if there was any potential outliers across all four treatment regimens.
##### - Created a grouped DataFrame that shows the last (greatest) time point for each mouse. Merged this grouped DataFrame with the original cleaned DataFrame.
##### - Created a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
##### - Looped through each drug in the treatment list, locating the rows in the merged DataFrame that corresponded to each treatment. Appended the resulting final tumor volumes for each drug to the empty list.
##### - Determined outliers by using the upper and lower bounds, and then printed the results.
##### 2.) Using Matplotlib, generated a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group.
![matplotlib5](https://github.com/kmorrow439/matplotlib_challenge/assets/114371722/01553aec-ac01-4c8a-b06a-e9eb1383f898)
---
#### Created a Line Plot and a Scatter Plot
##### 1.) Selected a single mouse that was treated with Capomulin, and generated a line plot of tumor volume versus time point for that mouse.
![matplotlib4](https://github.com/kmorrow439/matplotlib_challenge/assets/114371722/d0bf9e0a-db4b-4b3e-8c22-4e1c8b41b0bd)
##### 2.) Generated a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.
![matplotlib3](https://github.com/kmorrow439/matplotlib_challenge/assets/114371722/7fbba916-8723-4690-a991-1b332ec4682b)
---
#### Calculated Correlation and Regression
##### 1.) Calculated the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.
##### 2.) Plotted the linear regression model on top of the previous scatter plot.
![matplotlib1](https://github.com/kmorrow439/matplotlib_challenge/assets/114371722/b0834f01-401f-4104-bdab-9ecf1d914fb9)
