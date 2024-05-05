# COVID-19-Data-Analysis

## Project Overview

This analysis aims to evaluate the global progression of COVID-19, including its impact on specific continents and nations by examining the evolution of infection, recovery, and mortality rates. It seeks to identify critical periods of change, such as notable surges in case numbers or the efficacy of mass vaccination initiatives, to understand the dynamics of the pandemic's spread and control measures. An essential component of this research involves comparing the pandemic's impact across different geographical regions, to determine which areas have been disproportionately affected and the underlying causes. This comparison encompasses an analysis of case fatality rates, recovery rates, and the efficiency of testing among countries, thereby shedding light on the strategies adopted by governments and health organisations.

Furthermore, the study aims to investigate potential correlations between pandemic-related metrics, such as death and case rates and other variables, including testing rates and population size. This analysis aspect is intended to yield insights into the factors influencing the pandemic's trajectory. Additionally, the relationship between the number of serious or critical cases and overall death rates will be examined to assess the capacity and preparedness of healthcare systems in various regions.

Demographic factors will also be considered, specifically whether population size, both smaller and larger, affects the spread and mortality rates of COVID-19, incorporating an analysis of population density's role in virus transmission. Moreover, the effectiveness of testing strategies will be evaluated by analysing the number of tests conducted per one million population across different continents. This aspect of the analysis aims to understand the correlation between testing strategies and the identification of cases, providing unique insights into how early or widespread testing can influence pandemic management.

The comprehensive goal of this research is to chart the landscape of the COVID-19 pandemic and derive actionable insights that can inform policymaking and enhance the response to current and future public health crises.

This analysis utilised two datasets: the World Meter Coronavirus Daily Data and the World Meter Coronavirus Summary Data, which will be referred to as the Daily dataset and the Summary dataset, respectively. Both datasets were obtained from Kaggle. To access the original datasets, please follow this link: https://www.kaggle.com/datasets/josephassaker/covid19-global-dataset.

The summary dataset includes the following fields:

•	Country

•	Continent

•	Total Confirmed Cases

•	Total Deaths

•	Total Recovered

•	Active Cases

•	Serious or critical

•	Total cases per 1m population

•	Total deaths per 1m population

•	Total tests

•	Total tests per 1m population

•	Population

The daily dataset contains the following fields:

•	Date

•	Country

•	Cumulative Total Cases

•	Daily New Cases

•	Active Cases

•	Cumulative Total Deaths

•	Daily New Deaths

The two datasets encompass data from 266 countries, covering a period from January 22, 2020, to May 14, 2022, which spans 844 days or 2 years, 3 months, and 23 days.

The primary instrument employed for conducting this analysis was Microsoft Excel, along with its Data Analysis ToolPak. Microsoft Excel served as the foundational platform for organising, filtering, and analysing the data, while the Data Analysis ToolPak extension provided advanced statistical functions and analytical capabilities, enabling a more comprehensive exploration of the datasets. This combination of tools facilitated a robust and detailed data assessment, allowing for the efficient execution of various analytical tasks such as regression analysis, hypothesis testing, and data visualisation.

## Data Cleaning and Preparation

Both datasets were subjected to an exhaustive review for missing values, leveraging the find and select tools in Excel to detect blank cells within the datasets. All identified blank cells were then replaced with zeros, a critical modification given that each field could potentially harbour a value of zero. To further ensure data integrity, each column underwent a verification process to ascertain the proper data type was applied after missing values were addressed. Moreover, filters were applied across columns to confirm the elimination of any residual blank cells.

In the subsequent stage of data cleaning and preparation, a detailed examination confirmed the absence of outliers, thereby safeguarding the dataset's integrity and consistency. Such rigorous scrutiny was essential for improving the precision of further analyses. The presence of outliers could substantially distort findings and undermine the dependability of data-informed conclusions. This level of meticulousness in the initial stages of data processing significantly contributes to the robustness and reliability of the research outcomes.

## Exploratory Data Analysis

The Summary Dataset was analysed using the Descriptive Statistics function, which provided valuable insights. Various statistical measures were calculated and analysed, resulting in a comprehensive summary of the summary dataset as shown below:



The summary below was also obtained using the Descriptive Statistics functionality on the daily dataset:


The distribution of cases, deaths and recoveries across each continent was also part of the exploratory data analysis that was conducted as displayed in the visualisations below:

[Total Confirmed Cases Across Continents]

[Total recovered Cases Across Continents]

[Total Deaths Across Continents]

These graphs are indicative of the distribution of confirmed COVID-19 cases, fatalities, and recoveries across different regions of the world. The data reveals that Europe has been hit the hardest by the pandemic, with the highest number of confirmed cases, deaths, and recoveries. This trend can be attributed to factors such as high population density, extensive travel, and ease of transmission. Following Europe are Asia and North America, both of which have also experienced significant outbreaks. South America and Africa, on the other hand, have had relatively fewer cases and fatalities, although it is important to note that the numbers may be influenced by differences in testing capacity and reporting standards.

Overall, the graphs highlight the global impact of COVID-19 and underscore the need for continued efforts to mitigate the spread of the virus. These efforts include increased testing, contact tracing, social distancing, and vaccination campaigns. By working together, we can overcome this crisis and emerge stronger and more resilient than ever before—distribution of Cases, Deaths, and Recoveries Across Countries.

As in the prior segment, the exploratory data analysis continues to employ bar charts for visual representation. In this iteration, the charts serve to break down the Total Confirmed COVID-19 Cases, Total Recovered cases, and Total Deaths by country within the continents previously examined:

Africa:

x

x

x

Asia:

x

x

x


Australia:

x

x

x

Europe:

x

x

x

North America:

x

x

x


South America:

x

x

x

### Trends Over Time

The graphs presented show the worldwide cumulative and daily counts of COVID-19 cases, spanning from January 22, 2020, to May 14, 2022, which marks the most recent update of the dataset.

[Daily New COVID-19 Cases]

[Cumulative Total COVID-19 Cases]

The visualisations provided below display the cumulative and daily totals of COVID-19 cases on a global scale, encapsulated within the same date range as previously illustrated in the preceding two visualisations.

[Daily New COVID-19 Deaths]

[Cumulative Total COVID-19 Deaths]

This concluding visualisation illustrates the trajectory of active COVID-19 cases across the same period as the preceding visual representations:

[Active COVID-19 Cases]

## Comparative Analysis

### Cases, Deaths and Recovery Rates by Country and Continent

This analysis presents a comparison of COVID-19 metrics across various continents, examining Case Fatality Rate (CFR), Recovery Rate, Test Positivity Rate, Incidence Rate, and Testing Rate. Africa exhibits a CFR of 2.11% and a Recovery Rate of 84.18%, with a relatively high Test Positivity Rate of 11.79%, suggesting a higher proportion of positive cases among those tested. The continent's Incidence Rate and Testing Rate stand at 0.86% and 7.29%, respectively, indicating lower testing coverage compared to other regions.

Asia shows a lower CFR of 0.95% and a similar Recovery Rate to Africa at 84.10%. Its Test Positivity Rate of 7.08% and a significantly higher Testing Rate of 45.32% reflect broader testing efforts. The Incidence Rate in Asia is 3.21%, marking a moderate level of new case detection.

In Australia and Oceania, the lowest CFR of 0.14% is observed, alongside the highest Recovery Rate of 93.21%. This region also reports a high Test Positivity Rate of 9.98% and the largest Incidence and Testing Rates at 18.26% and 182.97%, respectively, indicating extensive testing and case detection efforts.

Europe presents a CFR of 0.94% and the second-highest Recovery Rate at 87.92%. The continent's Test Positivity Rate is 7.26%, with the highest Incidence and Testing Rates recorded at 25.96% and 357.48%, signifying widespread testing and infection.

North America's CFR stands at 1.47%, with the highest Recovery Rate among the regions at 95.17%. The Test Positivity Rate is 8.76%, and the Incidence and Testing Rates are 16.67% and 190.30%, respectively, reflecting substantial testing and recovery outcomes.

South America exhibits the highest CFR at 2.27% and a Recovery Rate of 89.31%, with a notably high Test Positivity Rate of 25.87%. This indicates a higher rate of infection among those tested. The Incidence Rate and Testing Rate are 13.06% and 50.50%, indicating moderate testing and case identification.

Globally, the CFR is 1.21%, with an average Recovery Rate of 88.35%. The worldwide Test Positivity Rate stands at 8.23%, with an Incidence Rate of 6.60% and a Testing Rate of 80.17%, showcasing a comprehensive overview of the pandemic's reach and response efforts across continents. This comparative analysis underlines the disparities in COVID-19 impact and response across different regions, underpinning the necessity for diverse strategies tailored to regional health infrastructures and epidemiological profiles.

The visualisations presented below provide a comprehensive summary of the analysis that had been carried out, encapsulating the key findings and insights derived from the data exploration:

[Case Fatality Rate by Continent]

[Recovery Rate by Continent]

[Positive Test Rate by Continent]

[Incidence Rate by Continent]

[Testing Rate by Continent]

## Critical Analysis

### Relationship between testing rates and confirmed cases.

This study conducted a linear regression analysis to investigate the relationship between the total number of COVID-19 confirmed cases (dependent variable, Y) and the total number of tests administered (independent variable, X) across 226 countries. The linear regression model aimed to predict the total confirmed cases of COVID-19 based on the number of tests administered within these countries. 

The results of the regression analysis revealed an Adjusted R Square value of 0.772352432, indicating that approximately 77.24% of the variability in the total confirmed COVID-19 cases can be explained by the linear relationship with the total tests administered. This high Adjusted R Square value suggests a strong explanatory power of the model. Furthermore, the Multiple R, or the correlation coefficient, was reported as 0.87941128, which implies a strong positive correlation between the number of tests administered and the confirmed COVID-19 cases.

The R Square value was calculated to be 0.773364199, nearly mirroring the Adjusted R Square and thus reinforcing the model's strength in terms of the explained variation. The regression model included an intercept of 524,208.061, indicating the expected number of confirmed cases when the total tests administered are zero. The slope of the regression line, or the coefficient for total tests, was 0.063568895. This coefficient suggests that for every additional test administered, there is an expected increase of approximately 0.063568895 in the number of confirmed COVID-19 cases.

Statistical significance for both the intercept and slope was assessed through p-values, with the intercept p-value recording at 0.036320039 and the coefficient p-value at an extremely low 3.78767E-74. These p-values indicate that both the intercept and the slope are statistically significant predictors of the total confirmed COVID-19 cases as shown in the visualisation below:

[Linear Regression Analysis: Relationship Between Total Tests and Confirmed Cases]

Additional statistical metrics provided in the analysis included the standard error of the regression, reported as 3,614,459.847, which provides a measure of the accuracy of predictions. The regression degree of freedom (DF) was 1, resounding the model's simplicity with only one predictor. The Sum of Squares due to Regression (SSR) was 9.98597E+15, with a Mean Square due to Regression (MSR) of the same value, reflecting the variability explained by the regression model. The F-statistic value was 764.3698841 with a Regression Significance F value of 3.78767E-74, attesting to the overall statistical significance of the regression model.

In conclusion, the linear regression analysis demonstrated a strong and statistically significant relationship between the total tests administered and the total confirmed cases of COVID-19 across 226 countries. The findings support the hypothesis that an increase in the number of tests administered is associated with an increase in the number of confirmed COVID-19 cases, revealing the critical role of widespread testing in the detection and management of the pandemic.

### Relationship Between Total Confirmed Cases and Population

This analysis investigates the relationship between the population of a country (X) and its total confirmed COVID-19 cases (Y) using a linear regression model. The dataset encompasses 226 observations corresponding to 226 countries, providing a unique lens through which to analyse this global health crisis.

The adjusted R-square value, which is 0.172936883, suggests that approximately 17.29% of the variance in the total confirmed COVID-19 cases can be explained by the country's population. This relatively low adjusted R-square value indicates a modest fit of the linear regression model to the data, hinting that other factors not considered in this model may significantly influence the total confirmed cases. The R-square value, closely aligned at 0.176612719, corroborates this interpretation, highlighting that a considerable portion of the variability in confirmed cases remains unaccounted for by population alone.

A multiple R, or the correlation coefficient, of 0.420253161, suggests a moderate positive correlation between the population and confirmed cases. This indicates that as the population increases, there is a tendency for the total confirmed cases to also increase, albeit not with strong predictability.

The regression analysis yields a line of best fit with a y-intercept (total tests Y Intercept) at 1,505,237.77 and a gradient (Line Gradient) of 0.022898253. This gradient implies that for every unit increase in population, there is an average increase of 0.022898253 units in the total confirmed COVID-19 cases, assuming all other factors remain constant as shown in the two visualisations below:

[Linear Regression Analysis: Relationship Between Population and Confirmed Cases]

[Linear Regression Analysis: Relationship Between Population and Confirmed Cases]

Moreover, the intercept and coefficient p-values (4.38474E-11 and 0.016388413, respectively) are significant indicators. The intercept p-value suggests that the model is statistically significant at predicting COVID-19 cases when the population is zero, despite this scenario not being practically feasible. The coefficient p-value denotes the significance of the population's effect on the total confirmed cases, affirming that the population does play a statistically significant role, albeit small, in influencing the COVID-19 case count.

The analysis also outlines the regression diagnostics with a regression degree of freedom (DF) of 1, a regression sum of squares (SS) of 2.28049E+15, a mean square (MS) of 2.28049E+15, and an F-statistic (Regression F) of 48.046952. The significance F (Regression Significance F) of 4.38474E-11 further supports the model's statistical significance. These diagnostics confirm the strength and significance of the regression model in explaining variability in confirmed COVID-19 cases as influenced by population while also identifying its limitations in accounting for all variances seen in the data.

In conclusion, this linear regression analysis provides evidence of a statistically significant, though modest, relationship between population size and confirmed COVID-19 cases across 226 countries. The model underscores the role of the population in predicting confirmed cases but also indicates the necessity of considering other factors to more comprehensively understand the dynamics of COVID-19 spread.

### Analysis of Death Rates

The analysis of the COVID-19 case fatality rate across 226 countries presents several noteworthy statistical insights into the distribution and variability of these rates. The mean fatality rate stands at 1.4%, indicating the average fatality ratio across the studied countries. However, the median of 0.97% is notably lower than the mean, which suggests a right-skewed distribution of fatality rates; this observation is further substantiated by a skewness value of 5.157862. The mode of the dataset is 0%, indicating that the most common fatality rate reported among the countries is 0%. This further implies that a significant number of countries have reported no or very low COVID-19 fatalities relative to their case counts, likely contributing to the skew.

The standard deviation, a measure of the dispersion of the fatality rates around the mean, is relatively small at 0.017319, supplemented by a standard error of the mean at 0.11%. This small standard deviation, in context with the relatively large range of 18.18% (with minimum and maximum values at 0% and 18.18%, respectively), suggests that while most countries have fatality rates clustered closely around the mean, there are outliers with significantly higher rates. This is further corroborated by the high kurtosis value of 41.59582, indicating a very peaked distribution with fat tails, hence a significant presence of outliers beyond the expectation of a normal distribution.

The sample variance of 0.0003 suggests a low variability in the case fatality rates across the sampled countries. However, the presence of outliers (as indicated by kurtosis) and the right-skewed nature of the distribution underscore the impact of countries with unusually high fatality rates on the overall statistical measures.

The sum of the case fatality rates in the dataset amounts to 3.187737, which, while providing a cumulative insight, yields more significance when viewed in conjunction with the count of 226 countries, offering a broader perspective on the global impact of COVID-19 in terms of fatality ratios.

A 95% confidence level with a margin of error at 0.23% points towards a high degree of certainty about the mean fatality rate estimate, indicating that were the sampling to be repeated, the mean fatality rate of the entire population would lie within this confidence interval 95 times out of 100. 

In conclusion, the statistical analysis reveals a generally low but highly variable COVID-19 case fatality rate across the studied nations, characterised by a significant right skew and a pronounced presence of outliers. This variability underscores the heterogeneity in the impact of the pandemic across different regions, likely influenced by factors such as healthcare capacity, demographic profiles, and the efficacy of public health interventions.

## Conclusion and Recommendations

In conclusion, the analysis of the two COVID-19 datasets, last updated in May 2022, provides valuable insights into the spread and impact of the pandemic across various regions. However, it is crucial to acknowledge the limitations inherent in the study due to the data's timeliness and comprehensiveness. A more recent dataset could potentially offer a more accurate and updated analysis of the pandemic's status and trends. Additionally, the presence of missing data from numerous countries significantly impacts the overall accuracy and reliability of the analysis conducted. These gaps in data not only hinder the ability to form a complete global picture but also affect comparative analyses between regions.

Several recommendations are proposed to enhance the quality and efficacy of future research. First, efforts should be made to acquire the most current data available, ensuring that analyses reflect the latest trends and developments in the pandemic's progression. This includes actively seeking updates from official and credible sources. Second, addressing the issue of missing data is paramount. Researchers should collaborate with international health organisations and local authorities to improve data collection and reporting processes. This may involve providing technical support or resources to countries struggling to collect or share data.

Furthermore, adopting advanced data imputation techniques could mitigate the impact of missing information. Though not without limitations, these methods can provide reasonable estimations that enable more comprehensive analyses. Finally, future studies should incorporate a more dynamic approach by analysing data in real-time or through short intervals. This approach will not only improve the accuracy of pandemic monitoring but also enhance the responsiveness of containment and mitigation strategies.

By adhering to these recommendations, future analyses can overcome the limitations observed in this study, thereby contributing to a more informed understanding of the pandemic and guiding effective policy-making and public health interventions.














