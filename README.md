# HR_Analytics

Introduction:

Employee turnover and dissatisfaction pose major challenges to organizations, increasing operational costs and reducing overall productivity. This project analyzes an HR dataset to identify key factors affecting employee satisfaction and performance, aiming to provide actionable insights to improve retention and boost workforce engagement.

This report aims to explore and analyse the dataset on HR. Let's delve into the details:

1. Data Overview:
   
•	The dataset consists of information about different Employees.

•	The dataset consists of information about employees, including satisfaction levels, last evaluation scores, number of projects, average monthly working hours, time spent at the company, work accidents, promotions in the last five years, department (sales, technical, support, etc.), salary level, and whether the employee left the company.


3. Data Acquisition and Preprocessing
   
The HR data was loaded from a CSV file using pandas. Libraries like NumPy and warnings were imported for numerical operations and handling warnings, respectively. seaborn, and matplotlib were used for data visualization.

Data cleaning steps included:

•	Handling missing values by replacing 'na' with NaN.

•	Replaced all occurrences of 'na', 'N/A', and blank entries with np.nan for proper handling.

•	Checked for missing values using isnull().sum(), and confirmed that the dataset was complete with no null values.

•	Renamed columns where necessary for better readability.


4. Exploratory Data Analysis (EDA)
   
•	Dataframe information and dtypes were explored using df.info() and df.dtypes.

•	Column names were retrieved using df.columns to understand the scope and variables available for analysis.

•	Distribution of key variables like satisfaction_level, last_evaluation, average_monthly_hours, and time_spent_company was analyzed.

•	Counts of categorical variables such as Work_accident, promotion_last_5years, Departments, and salary were plotted using bar charts.


5. Data Description
   
Descriptive statistics were generated for numerical columns to understand measures like mean, median, minimum, maximum, and standard deviation. Key observations included:

•	Satisfaction Level: Ranged between very low to very high with some clustering.

•	Last Evaluation: Concentrated towards the higher range (good evaluations).

•	Average Monthly Hours: Showed wide variation, indicating differences in workload.

•	Time Spent at Company: Majority employees had shorter tenures (2–4 years).


6. Attrition Analysis
    
•	Employees who left the company had lower satisfaction scores compared to those who stayed.

•	Employees with extremely high or low average_monthly_hours were more likely to leave.

•	A significant number of employees who left had low salaries compared to medium and high salary groups.

•	Departments like sales and technical had higher attrition rates compared to others.

•	Employees who received promotions in the last five years had lower attrition rates.


7. Data Visualizations
    
•	Histograms: Showed distribution of satisfaction levels, last evaluation scores, and monthly working hours.

•	Bar plots: Compared attrition rates across departments and salary levels.

•	Boxplots: Analyzed satisfaction levels and working hours in relation to attrition.

•	Heatmap: Revealed correlations between variables like satisfaction level, last evaluation, number of projects, and attrition.




Conclusion:

•	Lower employee satisfaction is strongly linked to higher turnover rates.

•	Employees with low salaries are more likely to leave compared to those with medium or high salaries.

•	Employees working extremely high or low monthly hours have a greater tendency to leave the organization.

•	Lack of promotion in the last five years is associated with increased employee attrition.

•	Departments like Sales and Technical experience higher turnover than others.

This report provides a foundational exploration of the HR dataset and identifies opportunities for HR managers to create targeted interventions. Future work can involve building predictive models for attrition prediction and conducting deeper segmentation analysis.
