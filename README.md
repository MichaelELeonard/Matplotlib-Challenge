<img src="Pics/Header.png" width="748" height="165">

# Pymaceuticals Inc.

##### Link to Matplotlib-Challenge code - https://github.com/MichaelELeonard/Matplotlib-Challenge/blob/main/pymaceuticals_working.ipynb
<br>

The task of this challenge was to complete the data analysis on a drug regimen to treat Squamous Cell Carcinoma (SCC), which is a form of skin cancer.  Pymaceuticals Inc. has a drug of interest for this treatment called Capomulin, so the study was conducted to see how Capomulin performed against other SCC drug options.  249 mice with SCC tumors received drug regimens to examine effects on their SCC tumor size.  The drugs in the study included: 
* Capomulin
* Ceftamin
* Infubinol
* Ketapril
* Naftisol
* Placebo
* Propriva
* Ramicane
* Stelasyn
* Zoniferol   

## DATA ASSEMBLY AND CLEANING
The first step in the process was to prepare and clean the data for analysis.  Two dataframes ‘mouse_metadata’ and ‘study_results’ were merged into a single dataframe ‘mice_data_complete.’  Each mouse subject was counted totaling 249.  A duplicate mouse ID ‘g989’ was identified and its data was removed from the data pool, so after cleaning the data the unique mouse count totaled 248.    
<br>  
<img src="Pics/mice_count.png" width="468" height="157">
<br>  
<img src="Pics/clean_mice_count.png" width="471" height="134">
<br>
<br>

## SUMMERY STATISTICS
Overall summary statistics were calculated examining the mean, median, variance, standard deviation & standard error of measurement of all the drug regimens in the trial.

<img src="Pics/tumor_summary.png" width="904" height="297">


These results were also replicated utilizing the aggregation method.  
<br>
<img src="Pics/tumor_summary_aggerate.png" width="473" height="296">
<br>
<br>



## BAR & PIE CHARTS
The cleaned dataframe was utilized to provide information for the next set for charts.  A bar chart was created to examine Mouse ID/Timeplots for each drug regimen.  This chart was created using both Pandas and pyplot.     
<br>
<img src="Pics/bar plot.png" width="475" height="408">


A pie chart was also created showing the Female vs. Male mice count utilized in the study.  This chart was also created using Pandas and pyplot.
<br>

<img src="Pics/pie plot.png" width="337" height="339">

## QUARTILES, OUTLIERS & BOXPLOTS
The data was then prepared to examine the specific results of Capomulin, Ramicane, Infubinol,
and Ceftamin.  This data was prepared for Boxplots by identifying the quartiles for each drug dataset.  A Boxplot graph was created for examination.
<br>
<br>
<img src="Pics/box plot.png" width="469" height="377">
<br>
<br>

## LINE AND SCATTER PLOTS
For the final analysis, the results of Capmulin was singularly examined.  A Line Plot was constructed to examine the SCC tumor size vs. the day point in the study and a Scatter Plot was used to show the relationship between SCC tumor size vs. the weight of the mice.
<br>
<br>
<img src="Pics/line plot.png" width="467" height="377">
<img src="Pics/scatter plot.png" width="467" height="377">
<br>
<br>


## CORRELATION AND REGRESSION
A Correlation and Regression line was added to the Scatter Plot to fully highlight the relationship between SCC tumor size vs. the weight of the mice.
<br>
<br>
<img src="Pics/linear regression.png" width="467" height="376">
<br>
<br>



## RESULTS
For this study, Pymaceuticals Inc. examined their drug of interest Capomulin vs. other drug regimens for the treatment of Squamous Cell Carcinoma (SCC) which is a form of skin cancer.  When looking at the Summary Statistics table, the tumor size of the Capomulin trial appears to be approximately 26% smaller than the eight other drug regimens in the study.  In the bar chart examining the timepoints throughout the study, Capomulin appears to be outperforming the other drug regimens in the study.  Utilizing a box plot to examine tumor size vs drug regimens, Capomulin showed promising results with a mean value in the high 30mm3.  The line plot also shows that Capomulin slowed tumor growth with a 8% reduction in overall tumor size from days 20 to 35.  Finally, the scatter plot with the correlation and regression overlay shows a strong positive correlation between tumor volume and subject weight.  In total, these initial trial studies highlight a potential positive upside for Capomulin in the treatment of Squamous Cell Carcinoma (SCC) and may warrant longer term studies on the efficacy of future Capomulin treatments.  

