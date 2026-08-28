# Research Results

This directory presents the main analytical results of the research on the capital mobilization and utilization of Vietnamese listed manufacturing enterprises during 2015–2023.

## Key Findings

### 1. Financial Performance

The dataset used in the financial performance analysis contains **3,274 observations**. The average ROA is **5.29%**, while the average ROE is **10.45%**. The observed ROA ranges from **-36.64% to 40.67%**, and ROE ranges from **-77.94% to 77.86%**, indicating substantial differences in financial performance across enterprises.

### 2. Capital Structure and Financial Indicators

The descriptive analysis reports an average **D/E of 1.219263**, indicating that debt is approximately 1.22 times equity on average. The average **LIQ is 0.201052**, while average **AT is 1.284830**. The average **SIZE is 27.105982** and average **Growth is 0.029251**.

### 3. Correlation Analysis

The Pearson correlation analysis shows a correlation of **0.8618 between ROA and ROE**. Among the explanatory variables, LIQ has a correlation of **0.2955 with ROA**, while AT and Growth have correlations of **0.2197** and **0.2221**, respectively. D/E has a negative correlation with ROA of **-0.2107**.

### 4. GLS Regression Results

The study estimates GLS models for ROA and ROE across two periods: **2015–2019** and **2020–2023**. The models include five explanatory variables: **AT, D/E, LIQ, SIZE, and Growth**.

For ROA, the coefficient of LIQ increases from **0.0661** in 2015–2019 to **0.0833** in 2020–2023. AT also increases from **0.0166** to **0.0197**, while SIZE increases from **0.0100** to **0.0136**. D/E remains negative, changing from **-0.0111** to **-0.0125**.

For ROE, AT remains positive and statistically significant, with coefficients of **0.0477** and **0.0486** in the two periods. D/E remains negative and becomes more pronounced after 2020, changing from **-0.0142** to **-0.0338**. LIQ changes from a negative and statistically insignificant coefficient of **-0.0042** before 2020 to a positive and statistically significant coefficient of **0.0493** after 2020.

### 5. Model Explanatory Power

The reported GLS results show that the R² of the ROA model increases from **0.213** in 2015–2019 to **0.275** in 2020–2023. For ROE, R² increases from **0.155** to **0.246**. The study notes that R² is not the primary evaluation criterion for GLS, as the main purpose of GLS is to address model deficiencies and obtain more efficient and reliable estimates.

## Main Research Implications

The reported results indicate a change in the role of liquidity after the COVID-19 period. LIQ shows a positive and statistically significant relationship with both ROA and ROE in 2020–2023, whereas its effect on ROE was negative and statistically insignificant in 2015–2019.

The results also show that **D/E has a negative relationship with both ROA and ROE in both periods**, with the negative effect on ROE becoming stronger after 2020. Meanwhile, AT, SIZE, and Growth generally show positive relationships with financial performance.

## Results File

### `research_results.docx`

Contains the extracted analytical results of the research, including:

* Capital mobilization analysis
* Capital utilization analysis
* Financial performance analysis
* Descriptive statistics
* Correlation analysis
* GLS regression results
* Supporting tables and figures
* Research discussion and recommendations

The document provides the detailed tables, figures, and interpretations underlying the summary presented above.

## How to Read the Project

For the overall research scope, objectives, methodology, and research framework, see [`PROJECT_OVERVIEW.md`](../PROJECT_OVERVIEW.md).

For the Python implementation and analytical workflow, see:

* [`01_exploratory_analysis.ipynb`](../notebooks/01_exploratory_analysis.ipynb)
* [`02_econometric_modeling.ipynb`](../notebooks/02_econometric_modeling.ipynb)

For information about the data source, scope, and variables, see [`../data/README.md`](../data/README.md).
