# Project Overview

## 1. Research Background

Capital mobilization and capital utilization are important aspects of financial management for manufacturing enterprises. This is particularly relevant to listed manufacturing enterprises, which operate in an environment characterized by increasing competition and changing financial conditions.

This study examines the capital mobilization and capital utilization of listed manufacturing enterprises in the Vietnamese stock market. It focuses on the selection of financing structures, the utilization of assets and liquidity, and the relationship between capital utilization and financial performance.

The study applies Python as a tool for quantitative financial analysis, with the aim of providing a broader perspective on capital management and supporting decision-making for enterprise managers and investors.

## 2. Research Objectives

The primary objective of this study is to provide a comprehensive view of how listed manufacturing enterprises in the Vietnamese stock market mobilize and utilize capital, and to provide useful information for enterprise managers and investors.

The study specifically aims to:

- Analyze important financial indicators related to capital utilization.
- Evaluate the efficiency of capital utilization through the relationship between financial indicators and business performance.
- Examine the relationship between capital-related factors and financial performance.
- Analyze the financing structure adopted by manufacturing enterprises, particularly the relative use of equity and debt financing.
- Provide directions for improving capital mobilization and capital utilization strategies to enhance financial performance.

## 3. Research Scope

### 3.1 Research Subjects

The study focuses on manufacturing enterprises listed on the three major Vietnamese stock exchanges:

- HOSE
- HNX
- UPCoM

### 3.2 Research Period

The study covers the period from **2015 to 2023**.

### 3.3 Data Source

The research data are derived from financial statements of listed manufacturing enterprises and were extracted from **FiinPro-X**.

## 4. Research Focus

The study examines three main aspects of capital management:

1. **Financing structure**  
   Analysis of the financing structure of manufacturing enterprises, including the relative use of equity and debt capital.

2. **Capital utilization**  
   Analysis of asset structure, liquidity, and indicators reflecting the utilization of capital and assets.

3. **Financial performance**  
   Analysis of the relationship between capital-related financial indicators and financial performance, measured primarily through **ROA** and **ROE**.

The study also examines these relationships across periods before and after the COVID-19 pandemic.

## 5. Variables

The main variables used in the quantitative analysis are:

| Variable | Description |
|---|---|
| ROA | Return on Assets |
| ROE | Return on Equity |
| AT | Total Asset Turnover |
| D/E | Debt-to-Equity Ratio |
| LIQ | Liquidity |
| SIZE | Firm Size |
| Growth | Firm Growth |

ROA and ROE are used to represent financial performance, while AT, D/E, LIQ, SIZE, and Growth are included as explanatory variables in the research model.

## 6. Research Methodology

The research follows a quantitative approach and applies Python for data processing, exploratory analysis, and econometric modeling.

### 6.1 Data Collection and Preparation

The dataset is constructed from financial data of listed manufacturing enterprises for the 2015–2023 period.

The data preparation process includes:

- Separating observations by year.
- Identifying observations with missing values.
- Removing observations that do not meet the specified data completeness criteria.
- Checking and removing outliers using the IQR statistical method.
- Standardizing data formats for subsequent analysis.

The Python implementation performs these data preparation steps before conducting the statistical and econometric analysis.

### 6.2 Descriptive and Exploratory Analysis

Descriptive analysis is conducted to examine the distribution and characteristics of the research variables.

The analysis considers:

- Mean
- Standard deviation
- Minimum and maximum values
- Percentiles

The exploratory analysis also examines capital structure, asset structure, liquidity, and financial performance across the research period and manufacturing sectors.

Pearson correlation analysis is subsequently used to examine the relationships among the variables and to identify potential multicollinearity concerns.

### 6.3 Panel-data Econometric Models

To examine the relationship between the explanatory variables and financial performance, the study estimates three panel-data models:

- **Pooled Ordinary Least Squares (Pooled OLS)**
- **Fixed Effects Model (FEM)**
- **Random Effects Model (REM)**

The models are applied to financial performance measures including ROA and ROE.

### 6.4 Model Selection and Diagnostic Testing

Model selection is conducted using statistical tests to determine the appropriate estimation approach.

The research applies:

- **F-test**
- **Hausman test**

The study also examines potential model specification issues through diagnostic testing, including:

- Variance Inflation Factor (VIF) for multicollinearity
- Breusch–Pagan test for heteroskedasticity
- Wooldridge test for serial correlation

### 6.5 Generalized Least Squares (GLS)

Following the diagnostic analysis, Generalized Least Squares (GLS) is applied to address model issues, particularly heteroskedasticity and serial correlation, with the aim of obtaining more reliable regression results.

The Python implementation constructs the GLS model using the estimated covariance structure derived from the residuals.

### 6.6 Period Analysis

In addition to the full research period, the study conducts separate analyses for:

- **2015–2019**
- **2020–2023**

This comparison is used to examine changes in the relationships between financial factors and financial performance across the two periods.

## 7. Key Descriptive Findings

The descriptive analysis indicates notable changes in the financial performance and financing structure of listed manufacturing enterprises over the research period.

During the pre-COVID-19 period, average ROE reached a peak of more than 20% in 2016 before declining in subsequent years. From 2018 to 2019, average ROE showed a slight recovery, although it remained below the levels observed during 2015–2016.

From 2020, ROA and ROE declined substantially as many enterprises experienced losses and faced difficulties in maintaining operating performance. ROA improved slightly in 2021 to approximately 4%, but the recovery was not sustained. During 2022–2023, ROA continued to decline and reached approximately 1% in 2023. :contentReference[oaicite:2]{index=2}

ROE reached a low of nearly 0% in 2020. It subsequently recovered to approximately 11% in 2021 before declining to approximately 9% in 2022 and 6% in 2023. :contentReference[oaicite:3]{index=3}

The financing structure also changed across the two periods. The debt ratio declined from 50.1% in 2019 to 47.3% in 2020, while equity increased to 52.7%. From 2021 onwards, the debt ratio increased again, reaching 48.9% in 2022 and 50.3% in 2023. :contentReference[oaicite:4]{index=4}

## 8. Correlation Analysis

The correlation matrix indicates a strong positive correlation between ROA and ROE, with a Pearson correlation coefficient of **0.8618**.

Asset turnover (AT) is positively correlated with both ROA (**0.2197**) and ROE (**0.2519**). Liquidity (LIQ) also shows a positive correlation with ROA (**0.2955**).

The correlation between D/E and ROA is negative (**-0.2107**), while its correlation with ROE is also negative (**-0.1303**).

The correlation matrix provides an initial overview of the relationships among the variables before proceeding to the econometric analysis. :contentReference[oaicite:5]{index=5}

## 9. GLS Regression Results

The final GLS estimation examines ROA and ROE across the two periods, 2015–2019 and 2020–2023.

| Variable | ROA<br>2015–2019 | ROE<br>2015–2019 | ROA<br>2020–2023 | ROE<br>2020–2023 |
|---|---:|---:|---:|---:|
| AT | 0.0166*** | 0.0477*** | 0.0197*** | 0.0486*** |
| D/E | -0.0111*** | -0.0142*** | -0.0125*** | -0.0338*** |
| LIQ | 0.0661*** | -0.0042 | 0.0833*** | 0.0493*** |
| SIZE | 0.0100*** | 0.0197*** | 0.0136*** | 0.0268*** |
| Growth | 0.0457*** | 0.0881*** | 0.0453*** | 0.0958*** |

The number of observations is 1,598 for the 2015–2019 models and 1,676 for the 2020–2023 models. The corresponding R² values are 0.213 and 0.155 for ROA and ROE in 2015–2019, and 0.275 and 0.246 in 2020–2023. :contentReference[oaicite:6]{index=6}

### Main Findings from the GLS Analysis

**Asset turnover (AT)** has a statistically significant positive effect on both ROA and ROE in both periods. Its coefficient increases from 0.0166 to 0.0197 for ROA and from 0.0477 to 0.0486 for ROE. The results indicate a stable positive relationship between asset utilization and financial performance. :contentReference[oaicite:7]{index=7}

**Debt-to-equity ratio (D/E)** has a negative and statistically significant coefficient across both financial performance measures and both periods. The results indicate a negative relationship between leverage and financial performance in the estimated models. :contentReference[oaicite:8]{index=8}

**Liquidity (LIQ)** has a positive and statistically significant relationship with ROA in both periods, with its coefficient increasing from 0.0661 to 0.0833. For ROE, LIQ is not statistically significant in 2015–2019 but becomes positive and statistically significant in 2020–2023. :contentReference[oaicite:9]{index=9}

**Firm size (SIZE)** has a positive and statistically significant relationship with both ROA and ROE in both periods. Its estimated coefficient increases for both dependent variables during 2020–2023. :contentReference[oaicite:10]{index=10}

**Growth** has a positive and statistically significant relationship with both ROA and ROE across both periods. Its coefficient remains positive and relatively stable for ROA while increasing for ROE during 2020–2023. :contentReference[oaicite:11]{index=11}

## 10. Implications

The research findings indicate the importance of effective capital and financial management for listed manufacturing enterprises.

The analysis highlights the role of liquidity, firm size, and asset turnover in the post-COVID-19 period. In particular, the coefficient of LIQ in the ROA model increases from 0.0661 to 0.0833, while the coefficients of SIZE and AT increase from 0.0100 to 0.0136 and from 0.0166 to 0.0197, respectively. :contentReference[oaicite:12]{index=12}

The results also indicate that enterprises need to maintain appropriate financial leverage. Excessive reliance on debt may increase interest expenses and financial risk, particularly in the manufacturing sector where enterprises typically hold substantial assets. The research therefore emphasizes the need for appropriate leverage and effective debt management. :contentReference[oaicite:13]{index=13}

For ROE, AT maintains a positive and statistically significant effect in both periods, while SIZE and Growth also show positive effects across the two periods. The report interprets these findings as evidence of the importance of asset management, firm scale, and sustained growth in supporting financial performance. :contentReference[oaicite:14]{index=14}

## 11. Conclusion

This study provides an empirical analysis of capital mobilization, capital utilization, and financial performance among Vietnamese listed manufacturing enterprises during 2015–2023.

Through descriptive analysis, correlation analysis, panel-data regression, model selection, diagnostic testing, and GLS estimation, the study examines the relationships between AT, D/E, LIQ, SIZE, Growth and the financial performance indicators ROA and ROE.

The analysis further distinguishes the periods before and after 2020, providing a basis for examining changes in the financial relationships of manufacturing enterprises across these periods.

The findings provide information relevant to the management of capital, assets, liquidity, and financial leverage, as well as to decision-making by enterprise managers and investors.
