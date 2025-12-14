# Term Project Data Analysis 2 and Assignment 2 Coding 2
---

## Project Structure

```
Final-Term-Project/
│
├── code/       # A jupyter notebook, which includes all data cleaning, analysis, and regression pipeline
├── data/       # all datasets used in this project
├── graphs/     # Generated plots
├── tables/       # Regression tables in LaTeX format
├── report/     # Final report (Markdown & PDF)
```

#### **Introduction**

This project is under the topic "Environment and Energy", and focuses on an important environmental and public health issue: urban air pollution. Understanding its causes is essential for effective policy-making and sustainable urban planning. While factors like industrial activity and vehicle emissions are often discussed, the roles of urban form characteristics, including population density and green space provision, are sometimes contested.

Therefore, this project studies the relationship between air pollution levels (measured by AQI) and three key urban variables in Chinese cities: (1) Population Density, (2) Green Coverage Rate, and (3) Industrial Land Ratio. We aim to find out these associations through regression analysis, and assess whether population density has a measurable link with air pollution.


#### **Data**

- **AQI-dataset_367_Chinese_cities_2014-2024**: The annual average AQI values for 367 cities across China. The Air Quality Index (AQI) is a comprehensive indicator used to assess air pollution levels, based on the concentrations of six major pollutants: PM2.5, PM10, SO₂, NO₂, O₃, and CO. 
Data Source: https://www.scidb.cn/en/detail?dataSetId=24ca93d08fdf4b9fa12842733caffe6d

- **Urban-area_square-kilometers**: The urban area data of cities across China.

- **Urban-construction-land-area_square-kilometers**: The total area of ​​urban construction land of cities across China, excluding undeveloped land area within the cities.

- **Urban-construction-land-area_Green-space-and-square-area_square-kilometers**: The total area of ​​land used for green spaces and squares within urban construction land. Squares are also included here, as squares typically include large areas of lawns and flowerbeds.

- **Urban-construction-land-area_Industrial-land_square-kilometers**: The total area of ​​industrial land within urban construction land.

- **Urban-population_in-ten-thousand**: The population data of cities across China.

The urban datasets above sourced from the *China Urban Construction Statistical Yearbook*.

- **city_translation**: An additional dataset for the English translations of all city names. The original datasets are downloaded from open websites of the statistical department of the Chinese government, and thus have column names in Chinese. By writing a Python script, we created this dataset as a Chinese-English glossary of Chinese city names, and merged it with all other datasets during the data preparation process.

By merging all datasets, we constructed a cross-sectional dataset including 313 city-level observations of the average values from 2017 to 2021.


