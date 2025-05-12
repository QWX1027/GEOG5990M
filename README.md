# GEOG5990M Assignment 2

# Investigating the Relationship Between Deprivation and Crime in Leeds

## Project Overview

This project explores the relationship between socio-economic deprivation and crime across neighbourhoods in Leeds, UK. Prior research suggests that deprived areas often experience higher crime rates, though the association may vary spatially and contextually.

Using publicly available spatial datasets, we conduct a reproducible analysis at the Lower Layer Super Output Area (LSOA) level. The workflow includes data preprocessing, statistical modelling, and geospatial visualisation using Python.

**Research Question**  
> Do more socio-economically deprived areas in Leeds report higher crime counts?

---

## Repository Contents

This repository contains all files needed to reproduce the analysis:

```
├── README.md                         ← Project documentation (this file)
├── crime_deprivation_analysis.ipynb  ← Main Jupyter Notebook with code and outputs
├── data/
│   ├── leeds_crime_March2025.csv     ← Crime data (March 2025, filtered to Leeds)
│   ├── leeds_imd_2019.csv            ← IMD 2019 scores for Leeds LSOAs
│   └── Leeds_LSOA_2011.zip           ← LSOA boundary shapefiles (zipped)
```

---

## Data Sources

- **Crime Data**  
  Downloaded from the [UK Police Data Portal](https://data.police.uk/data/).  
  File: `2025-03-west-yorkshire-street.csv` (filtered to Leeds)

- **Indices of Multiple Deprivation (IMD) 2019**  
  Source: 
[https://www.gov.uk/government/statistics/english-indices-of-deprivation-2019](https://www.gov.uk/government/statistics/english-indices-of-deprivation-2019)  
  File: `File_7_-_All_IoD2019_Scores__Ranks__Deciles_and_Population_Denominators_3.xlsx` (filtered to Leeds)

- **LSOA Boundaries (2011)**  
  [ONS Geography Portal](https://geoportal.statistics.gov.uk/)

---

## How to Run the Notebook

1. Clone or download this repository.
2. Ensure you have Python installed.
3. Install required packages (e.g., geopandas, matplotlib, seaborn, pandas).
4. Unzip `Leeds_LSOA_2011.zip` into the `data/` folder.
5. Open the `.ipynb` file in Jupyter Notebook, VS Code, or Google Colab.
6. Run all cells to reproduce the full analysis and visualisations.

---

## Method Summary

- **Exploratory Data Analysis**: Data pre-prcessing, data display (histograms, boxplots)
- **Statistical Modelling**: Pearson correlation, OLS linear regression
- **Mapping**: Choropleth maps for IMD Score and Crime Count using quantile classification
- **Software**: Python (pandas, geopandas, matplotlib, seaborn, statsmodels)

---

## Interpretation

- A weak but statistically significant positive correlation was found between deprivation and crime.
- Choropleth maps revealed overlapping spatial patterns, especially in central Leeds.
- The analysis supports the use of data-driven, place-based policy interventions.

---

## Reproducibility

This project was designed with reproducibility in mind. All data files, preprocessing steps, and analytical code are fully available in this repository. Others should be able to run the notebook and regenerate all results and maps.

---
