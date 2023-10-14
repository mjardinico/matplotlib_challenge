# Title: Module 5 Challenge (UC Berkeley Data Analytics Bootcamp 2023)
# Sub-title: pharmaceutical company specializes in anti-cancer medications
# Author:  Michael Jardinico
# version: 1.0
# Date created: 10/12/23

## Description: 
The file called pymaceutical_starter.ipynb is a study of a dataset of 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was obeserved and measured.  The purpose of this study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, against the other treatment regimens. 

The report is broken down into the following tasks:
    1. Prepare the data
    2. Generate summary statistics
    3. Create bar charts and pied charts
    4. Calculate quartiles, find outliers, and create a box plot
    5. Create aline plot and a scatter plot.
    6. Calculate correlation and regression.
    7. Submit final analysis.


# Dependencies
The script is written using Python 3.11 in Jupyter Notebook, although it may run using earlier versions of 3.x. The Python module and library used are Pandas, matplotlib.pyplot, numpy, scipy.stats. 

# Installing
1. Create a new repository for this project called matplotlib_challenge with README.md in GitHub
2. Clone the new repository to your computer.
3. Inside your local Git repository.
4. Inside matplotlib_challenge folder add a subfolder called data. 
5. Inside the data folder saved the two files:
   - Mouse_metadata.csv
   - Study_results.csv
   
# Getting Started
1. Open pymaceuticals_starter.ipynb in Jupyter Notebook.
2. Using pandas pd.read_csv to read both csv files (Mouse_metadata.csv and Study_results.csv) and assigned 
   them both to a variable
3. Merge the two data into a single DataFrame and name it mouse_study_complete, and display the table for 
   preview
4. Check the number of mice. In this example the result is 249
5. Remove duplicates using mouse ID and create a clean DataFrame and assign to a variable called 
   clean_mouse_study
6. SUMMARY STATISTICS:  create a summary statistics table of mean, median, variance, standard deviation, 
   SEM of the tumor volume for each regimen and assign to a variable called summary_statistic
7. Assemble the resulting series into a single summary DataFrame called summary_statistic.
8. Create a more advanced method to generate a summary of the statistic of table and assign to a variable
called summary_stats_adv
9. BAR AND PIE CHARTS: Group by Drug Regimen, Mouse ID, Timepoint in a DataFrame and call it 
drug_mouseid_df
10. Generate a bar plot showing the total number of rows (Mouse ID/Timpepoints) for each drug regimen using
Pandas
11. Generate a bar plot showing the total number of rows (Mouse ID/Timepoints) for each drug regimen using
pyplot. 
12. Generate a pie plot showing the distribution of female versus male mice using Pandas
13. Generate a pie plot showing the distribution of female versus male mice using pyplot. Note: the graph
should be similar to step# 12
14. QUARTILES, OUTLIERS AND BOXPLOTS: 
   - Calculate the final tumor volume of each mouse across fouur of the treatment regimens: Capomulin, Ramicane, Infubinol and Ceftamin.
   - Start by gettting the last (greatest) timepoint for each mouse
   - Merge this group df with the origina lDataFrame to get the tumor volume at the last timepoint.
   - Put treatments into a list for for-loop to be plotted 
   - Calculate the IQR and guantitatively determine if there are any potential outliers
   - Determine outlies using upper and lower bounds
   
15. Generate a box plot that shows the distribution of the tumor volme for each treatment group.
16. LINE AND SCATTER PLOTS: 
   - Generate a line plot for tumor volume vs. time point for a single mouse treated with Capomulin
   - Generate a scatter plot of mouse weight vs. the average observed tumor volume for the entire Capomulin regimen
   - Filter data for the Capomulin regimen
   - Show the Scatter plot
17. CORRELATION AND REGRESSION: 
   - Calculate the correlation coefficient and a linear regression model for the mouse weight and average
   observed tumor volume for the entire Capomulin regimen
   - Create the Scatter Plot and regression line

*** END OF CHALLENGE ***