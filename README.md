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























