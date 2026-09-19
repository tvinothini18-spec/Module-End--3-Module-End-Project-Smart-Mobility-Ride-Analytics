# Smart Mobility & Ride Analytics

## Project Overview

This project analyzes ride-hailing data to understand pricing, demand, customer ratings, peak-hour behavior, and potential fare anomalies. Statistical and mathematical techniques are applied to identify relationships between operational factors and business performance.

The analysis is based on a dataset containing **200 ride records**.

## Objectives

The main objectives of this project are to:

1. Determine whether trip distance significantly affects fare amount.
2. Compare fare amounts between Premium and Economy rides.
3. Analyze the relationship between surge pricing and customer ratings.
4. Compare Peak and Non-Peak ride revenue/fare amounts.
5. Detect unusual fare values and possible pricing anomalies.
6. Estimate ride-category demand probabilities.
7. Identify operational factors related to business performance.
8. Use statistical evidence to support pricing and service improvement decisions.

## Dataset

**File:** Trip_Analysis.xlsx

The dataset contains ride-level information including variables related to:

- Trip distance
- Fare amount
- Ride category
- Surge multiplier
- Customer rating
- Peak/Non-Peak ride timing

## Technologies and Libraries

The analysis can be implemented using:

- Python
- Jupyter Notebook / Google Colab / VS Code
- NumPy
- Pandas
- SciPy
- Matplotlib
- Seaborn
- Statistics

## Statistical Methods Used

### Descriptive Statistics
- Mean
- Median
- Standard deviation
- Quartiles
- Percentiles
- Variance

### Correlation Analysis
- Pearson correlation
- Spearman correlation
- Covariance

### Hypothesis Testing
- Independent-samples t-test
- One-way ANOVA
- Significance testing using p-values

### Anomaly Detection
- IQR method
- Z-score
- Quartiles
- Percentiles

### Probability Analysis
- Basic probability
- Conditional probability
- Bayes' theorem

### Advanced Analysis
- Confidence intervals
- Bootstrapping
- Linear regression
- Eigenvalue analysis
- Linear algebra interpretation

## Key Findings

### 1. Trip Distance vs Fare

Pearson correlation was approximately **0.017** with a p-value of **0.813**.

**Conclusion:** There is no statistically significant relationship between trip distance and fare amount in this dataset.

### 2. Premium vs Economy

Average fares were approximately:

- Economy: **₹257.75**
- Premium: **₹252.46**

The t-test produced a p-value of approximately **0.685**.

**Conclusion:** Premium rides were not statistically more expensive than Economy rides.

### 3. Surge Pricing vs Customer Rating

Spearman correlation was approximately **−0.047**, with a p-value of approximately **0.508**.

**Conclusion:** There is no statistically significant relationship between surge pricing and customer ratings.

### 4. Peak vs Non-Peak Rides

The Peak vs Non-Peak fare comparison produced a p-value of approximately **0.552**.

**Conclusion:** There is no statistically significant difference in fare revenue between Peak and Non-Peak rides.

### 5. Fare Anomalies

The IQR method identified **one potential fare outlier**. However, no observation exceeded the ±3 standard-deviation z-score threshold.

**Conclusion:** The potential outlier should be investigated rather than automatically removed.

### 6. Ride Demand Probabilities

Observed ride-category proportions:

| Ride Category | Count | Probability |
|---|---:|---:|
| Economy | 82 | 41% |
| Shared | 60 | 30% |
| Premium | 58 | 29% |

**Conclusion:** Economy rides represented the largest proportion of rides in the sample.

## Recommendations

1. Do not rely on trip distance alone when determining fare prices.
2. Review Premium and Economy pricing using additional operational variables before making major pricing changes.
3. Continue monitoring surge pricing and customer ratings.
4. Investigate the identified fare anomaly for possible data-entry or pricing errors.
5. Use observed ride-category probabilities for initial driver and vehicle allocation planning.
6. Collect additional variables such as waiting time, traffic conditions, pickup/drop-off location, vehicle type, driver availability, and demand level.
7. Use multiple regression, confidence intervals, bootstrapping, and A/B testing for stronger pricing and service decisions.

## Overall Conclusion

The analysis shows that the tested operational variables have **weak statistical relationships with fare amount and customer ratings**. None of the major tested relationships was statistically significant at the 5% significance level.

The dataset provides a useful baseline for ride analytics, but additional operational data is required to build more reliable pricing, demand, and service-performance models.

## Project Structure


Smart-Mobility-Ride-Analytics/
│
├── Trip_Analysis.xlsx
├── Smart_Mobility_Ride_Analytics.ipynb
├── README.md
└── requirements.txt


## How to Run

1. Download or clone the project.
2. Place `Trip_Analysis.xlsx` in the project folder.
3. Open the Jupyter Notebook in Google Colab, Jupyter Notebook, or VS Code.
4. Install the required Python libraries.
5. Run the notebook cells sequentially.
6. Review the statistical results, visualizations, and conclusions.

## Author
Vinothini
Aspiring Data Scientist

Focus Areas: Data Cleaning, Exploratory Data Analysis, Probability, Statistics, Linear Algebra, Hypothesis Testing, and Business Analytics.
