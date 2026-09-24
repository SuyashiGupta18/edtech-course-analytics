**# EdTech Course Analytics**



A data analytics project exploring what drives course completion and dropout

on a synthetic online course platform, using Python/pandas for cleaning and

exploration, and Power BI for an interactive dashboard.



**## Dataset**

1,500 student records (after cleaning) with demographics, course info,

engagement metrics, and outcomes (completion, dropout, ratings).



**## Tools Used**

\- Python (pandas, matplotlib, seaborn) in Google Colab

\- Power BI Desktop



**## Data Cleaning**

\- Handled 7 columns with missing values (imputed numeric fields with median,

&#x20; categorical fields with "Unknown"; left quiz\_avg\_score/rating as NaN where

&#x20; missing meant "not attempted"/"not started")

\- Removed 15 duplicate rows

\- Standardized 19 messy category label variants into 8 clean categories

\- Fixed a mixed text/numeric column and split it into a numeric score + flag

\- Corrected outliers (impossible ages, an inconsistent time-spent value)



**## Key Insights**

1\. \*\*Time spent is the strongest driver of completion\*\* — completers average

&#x20;  \~27 hours vs. \~2 hours for students who never start.

2\. \*\*Data Science has a completion bottleneck\*\*, not an engagement problem —

&#x20;  normal time spent and quiz scores, but the highest dropout rate (\~5x others)

&#x20;  and 79% of its students stuck "In Progress."

3\. \*\*Price and age don't meaningfully affect outcomes\*\* — both show near-zero

&#x20;  correlation with completion.

4\. \*\*Quiz participation and ratings are the strongest numeric predictors\*\* of

&#x20;  completion (0.73 and 0.60 correlation respectively).

5\. \*\*The platform's core challenge is stalled engagement, not dropout\*\* — 79%

&#x20;  of all students are "In Progress," while explicit dropout is rare (1-5%).



**## Files**

\- `notebook/` — Full analysis notebook (cleaning, exploration, visualizations)

\- `data/` — Raw and cleaned datasets

\- `dashboard/` — Interactive Power BI dashboard (.pbix)



## Dashboard Preview

![Power BI Dashboard](Images/Screenshot_dashboard_1.0.png)

![Power BI Dashboard](Images/Screenshot_dashboard_2.0.png)

## Key Charts

![Dropout Rate by Category](Images/barchart_dropout_rate.png)

![Correlation Heatmap](Images/Heatmap_correlation.png)

![Average Time spent](Images/barplot_avg_timespent.png)

![Completion per percent](Images/hist_comp_percentage.png)

![Completion Status](Images/Piechart_completion_status.png)





