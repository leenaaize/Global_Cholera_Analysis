## Global Cholera Trends: A Statistical Analysis

### PROBLEM STATEMENT
Despite global initiatives aiming to reduce cholera mortality to below 1%, the disease remains a significant public health threat.  This project seeks to uncover the patterns and trend of the cholera disease over time and to answer the question: Is there a measurable decline in the severity of outbreaks over time, and is geography a definitive factor in an individual's chance of survival?

### WHY IS THIS PROBLEM IMPORTANT
Cholera is a disease of inequity, acting as a marker of poverty, lack of social development, and inadequate access to basic services. Understanding where the disease is most lethal allows for the strategic allocation of resources. By analysing this dataset, we can identify the most vulnerable populations and  the regions that require more aggressive public health interventions

### DESCRIPTION OF DATASOURCE
The dataset is a WHO cholera dataset (sourced from Kaggle), covering global cholera surveillance data from 1949 to 2016.
Key Variables of Interest:
-	Year
-	Country
-	WHO Region
-	No. of Cases; how quickly the disease is spreading(incidence)
-	No. of Deaths; the total burden
-	Case Fatality Rate (CFR); severity of an outbreak

### ANALYTICAL OBJECTIVES
This analysis aims to 
-	Baseline Characterization: Establish the cumulative global burden and identify outlier years and regions of extreme epidemic activity.
-	Trend Assessment: Determine if the global volume of cases and mortality is increasing, decreasing, or stagnating over the 67-year period.
-	Hypothesis Testing: Statistically compare the Case Fatality Rate (CFR) between  regions to identify disparities in outbreak lethality.

### STATISTICAL METHODS USED
-	Descriptive Statistics
-	Time Series Analysis
-	Inferential Statistics
  
### METRICS 
-	Mortality (Total Deaths)
-	Prevalence (Total Cases)
-	Time Trend (Year)
-	Geographic Location (Country/Region)
-	Severity Indicator (Case Fatality Rate)
-	Descriptive Statistics: Cumulative totals, Medians, and Interquartile Ranges (IQR)
-	Trend Analysis 
-	Inferential Testing
  
### RISKS AND CONSTRAINTS
-	Historical under-reporting: there is a risk that older records are not as accurate as modern ones in certain regions may bias results. 
-	Geographical reporting standards: Reporting standards vary greatly by region. Some countries might report every single case, while others might only report cases that reach a hospital.
-	Data Skewness: public health data for diseases like cholera frequently tend to have a skewed distribution. We expect to see a few years with massive outbreaks and some with few cases.
-	Lack of demographic detail: The dataset provides totals counts but does not break down the data by age, gender, or specific location within a country. This is a constraint because we can identify where and when an outbreak happened, but we cannot see who was most affected, which limits specific healthcare recommendations.



