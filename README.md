## 📌 Life Expectancy Project: Analysis of Health and Immunizations

📅 Date: October 27, 2024

### 📖 Project Overview

This project explores the relationship between vaccination rates and life expectancy at the country level using data from the 2020 United Nations Human Development Report. We analyze whether higher immunization rates (DTP & measles vaccines) correlate with longer life expectancy using statistical modeling and visualization techniques in R.

### 🔍 Key Research Question:
 Do higher vaccination rates correlate with increased life expectancy?

### 📂 Repository Structure
📦 Life-Expectancy-Project │── 📁 dataset/ # Raw and cleaned data files

│── 📜 Life_Expectancy.Rmd # R Markdown analysis script

│── 📜 Life_Expectancy.html # HTML report from R Markdown

│── 📜 Life Expectancy Presentation.pptx # Project presentation

│── 📜 Project.Rproj # R Project file

│── 📜 README.md # Project documentation (this file)

### 📊 Data & Key Variables

- **Dataset:** United Nations Human Development Data (2020)  
- **Key Variables:**
  - `life` – Life expectancy at birth (years)  
  - `dtp_vax_no` – Number of DTP vaccinations per 100 population  
  - `measles_vax_no` – Number of measles vaccinations per 100 population  
  - `pop` – Total population  
- **Preprocessing Steps:**
   - Removed missing values
   - Converted non-numeric values to NA
   - Stored cleaned data in /dataset/

### 📈 Exploratory Data Analysis

- Visualizations Include:
- Scatter plots for vaccination rates vs. life expectancy
- Histograms for the distribution of vaccination rates
- Correlation analysis between key variables

### Findings:

Vaccination rates show unexpected trends in relation to life expectancy.
The distributions of DTP and measles vaccines are right-skewed, requiring log transformation for regression analysis.

###  Regression Analysis

1️⃣ Simple Linear Regression:
Examined DTP and measles vaccination rates separately in predicting life expectancy.

2️⃣ Multiple Linear Regression:
Included additional socioeconomic factors such as urbanization, fertility rate, tuberculosis incidence, GDP, and education levels.

### Key Results:

Higher fertility rates & tuberculosis incidence negatively impact life expectancy.
Education & food security show positive correlations with life expectancy.
Unexpectedly, higher vaccination rates correlated with slightly lower life expectancy, likely due to confounding variables.
---

## 🔧 How to Run the Analysis  
📌 Install the following R packages before running the scripts:  

```r
install.packages(c("ggplot2", "dplyr", "readr", "corrplot"))
