## Global Cholera Trends: A Statistical Analysis

### PROBLEM STATEMENT
This project seeks to uncover the patterns and trend of the cholera disease over time and to answer the question: Is there a measurable decline in the severity of outbreaks over time, and is geography a definitive factor in an individual's chance of survival?

### WHY IS THIS PROBLEM IMPORTANT
Despite global initiatives aiming to reduce cholera mortality to below 1%, the disease remains a significant public health threat. Cholera is a disease of inequity, acting as a marker of poverty, lack of social development, and inadequate access to basic services. Understanding where the disease is most lethal allows for the strategic allocation of resources. By analysing this dataset, we can identify the most vulnerable populations and  the regions that require more aggressive public health interventions

### ANALYTICAL OBJECTIVES
- Baseline Characterization: Establish the cumulative global cases and deaths. Summarise the central tendency and spread of Case Fatality Rates for different regions. Identify extreme outlier events and regions where they occured.
-	Trend Assessment: Determine if the global volume of cases and deaths is increasing, decreasing, or stagnating over the 67-year period.
-	Statistical Inference: Compare the Case Fatality Rate (CFR) across regions to identify significant disparities in outbreak lethality.


### METHODOLOGY
1. Data Acquisition & Source
   - Source: The dataset is a World Health Organization (WHO) cholera dataset (sourced from Kaggle), covering global cholera surveillance data from 1949 to 2016.
   -  Dataset: Global cholera cases, deaths and fatality rates spanning 1949-2016 across various countries and regions.
   -  Key Variables:
       - No. of Cases
       - No. of Deaths
       - Case Fatality Rate (CFR),the primary metric used to evaluate regional outbreak severity

2. Data Wrangling & Preprocessing
   - Cleaning: Handled inconsistent reporting standards and missing values inherent in long-term historical datasets.
   - Feature Engineering: Calculated and standardized Case Fatality Rates (CFR) to allow for fair comparisons across regions with vastly different infection volumes.
   - Filtering: Focused the analysis on the six primary WHO regions to ensure geographical relevance.
   - Data Validation: 

3. Exploratory Data Analysis
   - Performed descriptive statistics to summarize central tendency and spread of data.
   - Utilized Time-Series Analysis to identify global trends and "Black Swan" events (outbreak spikes).
   - Used Distributional Analysis (Boxplots) to compare regional survival disparities and identify outliers.
  
4. Inferential Statistics
   - Kruskal-Wallis Test: Applied as a non-parametric alternative to ANOVA, accounting for the skewed nature of epidemiological data.
   - Dunn’s Post-Hoc Test: Conducted to pinpoint exactly which regional pairs exhibited statistically significant differences in survival.

5. Tools & Environment
   -  Language: Python
   -  Libraries: Pandas(data manipulation), Seaborn/Matplotlib (visualization), Scipy/Scikit-posthocs (statistical testing).

  
### INSIGHTS
1. The Geography of Survival
- Location as a Determinant: Statistical evidence confirms that an individual’s geographical location is a definitive factor in their chance of survival. The lethality gap between the various regions is structural and statistically significant.

- Volume vs. Lethality: A major finding of this study is the decoupling of infection numbers from mortality risk. While Africa carries the highest volume of cases, South-East Asia has historically faced the highest mortality risk.

- Shared Vulnerability: Despite differences in scale, inferential testing proves that Africa and South-East Asia share a statistically identical high-risk profile.

2. A Global Success Story
- Effective Interventions: Trend analysis from 1949 to 2016 reveals that global medical interventions are working. Even as cases reached record highs in the 1990s and 2010s, mortality rates did not follow, proving we are becoming better at keeping people alive even as the disease spreads.

### RECOMMENDATIONS
- Public health policy should prioritize regions with high Case Fatality Rates (CFR) rather than just those with high case counts. High lethality indicates a more urgent need for immediate clinical support and resource allocation.

- Since survival is tied to geography, the challenge is logistical and structural. Global health initiatives must prioritize long-term infrastructure improvements in water and sanitation (WASH) alongside reactive medical treatment.
  
### LIMITATIONS & FUTURE WORK
1. Study Limitations
 -	Historical under-reporting: there is a risk that older records are not as accurate as modern ones in certain regions.
 -	Reporting Disparities: The 67-year historical range (1949–2016) carries a risk of under-reporting, particularly in older records or in regions where data capture is limited to hospital-based cases rather than community outbreaks.
 -	Lack of Demographic Detail: The dataset provides geographical totals but lacks granularity regarding age and gender. This prevents the identification of high-risk demographic groups and limits the ability to suggest specific interventions like age-targeted vaccinations.
 -	Data Skewness: Epidemiological data is naturally skewed by massive singular outbreaks; while our statistical tests accounted for this, these "Black Swan" events can sometimes mask long-term underlying stability.

2. Future Research
   - Socio-Economic Integration: Future analysis should aim to integrate localized socio-economic data (GDP per capita or infrastructure access) to model the specific drivers behind the regional gap.
   - Predictive Analysis: Moving beyond descriptive statistics to Machine Learning forecasting could help predict which regions are most likely to experience the next major fatality spike.
   - Localized Deep-Dives: Transitioning from WHO regions to country-level analysis to identify specific national success stories or infrastructure failures.
