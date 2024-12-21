# HIA302/322 Group Project
## Title: Descriptive Statistics of COVID-19 Death in Malaysia from 1 April 2021 to 30 November 2024
### COVID-19 data files extracted 
(from MoH-Malaysia/covid19-public)
+ deaths_malaysia.csv: Daily deaths due to COVID-19 at country level.
+ linelist_deaths.csv: List containing relevant clinical, demographic and vaccination information for each death reported.
### Population data files extracted
(from Department of Statistics Malaysia - https://pqi.stats.gov.my/searchBI.php)
+ AgePopulationByYear.csv: Annual population data by age groups at country level between year 2021 and year 2024.
+ GenderPopulationByYear.csv: Annual population data by gender at country level between year 2021 and year 2024.
### Data files created
+ deaths_trend.csv: data for analysis of deaths trend
+ deaths_vaccination_status.csv: data for analysis of deaths by vaccination status
+ deaths_demographic.csv: data extracted from linelist_deaths with columns of interest
+ deaths_age.csv: data for analysis of deaths by age groups
+ deaths_gender.csv: data for analysis of deaths by gender
+ deaths_comorbidity.csv: data for analysis of deaths by comorbidity status
## Metadata for Variables
### deaths_trend.csv
1. year_month: yyyy-mm format
2. deaths_new: monthly deaths due to COVID-19 reported in year_month 
3. total_pop: annual total population
4. year: yyyy format
5. death_rate: monthly death rate per 100,000 population
6. cumulative_deaths: successive addition of monthly deaths due to COVID-19
### deaths_vaccination_status.csv
1. year_month: yyyy-mm format
2. deaths_unvax: monthly number of unvaccinated individuals who died due to COVID-19 reported in year_month
3. deaths_pvax: monthly number of partially-vaccinated individuals who died due to COVID-19 reported in year_month
4. deaths_fvax: monthly number of fully-vaccinated individuals who died due to COVID-19 reported in year_month
5. deaths_boost: monthly number of individuals with at least 1 booster dose who died due to COVID-19 reported in year_month
### death_demographic.csv
1. date_announced: date on which the death was announced to the public
2. age: age as an integer; note that it is possible for age to be 0, denoting infants less than 6 months old
3. male: binary variable with 1 denoting male and 0 denoting female
4. comorb: binary variable with 1 denoting that the individual has comorbidities and 0 denoting no comorbidities declared
5. year: yyyy format, extracted from date_announced
6. year_month: yyyy-mm format, extracted from date_announced
7. age_group: 0-9 years, 10-19 years , 20-59 years and 60+ (60 and above) years
### deaths_age.csv
1. year_month: yyyy-mm format
2. age_group: 0-9 years, 10-19 years , 20-59 years and 60+ years 
3. Deaths: monthly deaths due to COVID-19 reported in year_month for each age_group
4. year: yyyy format
5. population: annual population for each age_group
6. Death Rate (per 100,000): monthly death rate per 100,000 for each age group
### deaths_gender.csv
1. year_month: yyyy-mm format
2. Male Deaths: monthly male deaths due to COVID-19 reported in year_month
3. Female Deaths: monthly female deaths due to COVID-19 reported in year_month
4. Total Deaths: monthly sum of male and female deaths
5. year: yyyy format
6. total_pop: annual total population
7. pop_male: annual male population
8. pop_female: annual female population
9. Male Death Rate: monthly male death rate per 100,000
10. Female Death Rate: monthly female death rate per 100,000
### deaths_comorbidity.csv
1. year_month: yyyy-mm format
2. Deaths with comorbidities: monthly deaths with comorbidities due to COVID-19 reported in year_month
3. Deaths without comorbidities: monthly deaths without comorbidities due to COVID-19 reported in year_month
4. Total Deaths: monthly sum of deaths with comorbidities and deaths without comorbidities
