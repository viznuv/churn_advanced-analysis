# Telecom Customer Churn Analysis

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![lifelines](https://img.shields.io/badge/lifelines-0.27.0-green)
![scikit--learn](https://img.shields.io/badge/scikit--learn-1.0%2B-orange)
![Pandas](https://img.shields.io/badge/pandas-1.3%2B-yellow)
![Matplotlib](https://img.shields.io/badge/matplotlib-3.5%2B-red)
![Seaborn](https://img.shields.io/badge/seaborn-0.11%2B-blue)

![image](https://github.com/user-attachments/assets/e48e5d76-73ff-42a5-aa5a-be3f89a6f4f5)

## 📊 Comprehensive Telecom Customer Churn Analysis with Survival Analytics

This repository contains a comprehensive Python-based analytics toolkit for analyzing customer churn in the telecommunications industry using advanced survival analysis techniques. The script performs in-depth analysis of customer behavior, churn patterns, and lifetime value using both classical machine learning and specialized survival analysis methods.

## ✨ Features

- **Comprehensive EDA**: Detailed exploratory data analysis of telecom customer data
- **Predictive Modeling**: Machine learning models to predict customer churn
- **Survival Analysis**: Kaplan-Meier survival curves and hazard analysis
- **Cox Proportional Hazards Modeling**: Identify factors affecting customer churn risk
- **Parametric Survival Models**: Log-normal, Weibull, and Exponential survival models
- **Customer Lifetime Value**: Calculate and analyze CLV across customer segments
- **Cohort Analysis**: Track churn patterns across different customer cohorts
- **Data Visualization**: Rich visualizations of all analysis results
- **Strategic Recommendations**: Data-driven insights for reducing churn

![image](https://github.com/user-attachments/assets/c4a2e987-5ddb-47d3-9d4c-806802255ad7)

## 📋 Dataset Description

The analysis is designed for telecom customer datasets with the following structure:

| Field | Description |
|-------|-------------|
| customerID | Unique customer identifier |
| gender | Customer gender (Male/Female) |
| SeniorCitizen | Whether customer is a senior citizen (0/1) |
| Partner | Whether customer has a partner (Yes/No) |
| Dependents | Whether customer has dependents (Yes/No) |
| tenure | Number of months customer has been with the company |
| PhoneService | Whether customer has phone service (Yes/No) |
| MultipleLines | Whether customer has multiple lines (Yes/No/No phone service) |
| InternetService | Customer's internet service provider (DSL/Fiber optic/No) |
| OnlineSecurity | Whether customer has online security (Yes/No/No internet service) |
| OnlineBackup | Whether customer has online backup (Yes/No/No internet service) |
| DeviceProtection | Whether customer has device protection (Yes/No/No internet service) |
| TechSupport | Whether customer has tech support (Yes/No/No internet service) |
| StreamingTV | Whether customer has streaming TV (Yes/No/No internet service) |
| StreamingMovies | Whether customer has streaming movies (Yes/No/No internet service) |
| Contract | The contract term of the customer (Month-to-month/One year/Two year) |
| PaperlessBilling | Whether customer has paperless billing (Yes/No) |
| PaymentMethod | The customer's payment method |
| MonthlyCharges | The amount charged to the customer monthly |
| TotalCharges | The total amount charged to the customer |
| Churn | Whether the customer churned (Yes/No) |

## 📦 Requirements

- Python 3.7+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- lifelines
- scipy

## 🔧 Installation & Setup

1. Clone this repository:
```bash
git clone https://github.com/yourusername/telecom-churn-analysis.git
cd telecom-churn-analysis
```

2. Create a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install the required packages:
```bash
pip install -r requirements.txt
```

## 📊 Usage Instructions

### Using Google Colab

1. Upload the `telecom_churn_analysis.py` script to Google Colab
2. Upload your CSV data file to Colab or mount Google Drive
3. Update the file path in the script to point to your data
4. Run all cells to execute the complete analysis

### Running Locally

1. Place your telecom customer data in a CSV file in the project directory
2. Update the file path in the script to point to your data:
```python
# Replace with your file path
df = pd.read_csv('your_file.csv')
```
3. Run the script:
```bash
python telecom_churn_analysis.py
```
![image](https://github.com/user-attachments/assets/24f4bbf6-f4ac-4dbe-b0c2-df1075dfc4db)

## 🔬 Analysis Components

The analysis is structured into the following sections:

1. **Data Loading & Exploration**
   - Basic data inspection
   - Data cleaning and preprocessing
   - Summary statistics and distributions

2. **Exploratory Data Analysis (EDA)**
   - Churn distribution visualization
   - Feature distribution analysis
   - Correlation analysis
   - Demographic and service usage patterns

3. **Predictive Churn Modeling**
   - Random Forest classification
   - Feature importance ranking
   - Model performance evaluation
   - ROC curve analysis

4. **Survival Analysis**
   - Kaplan-Meier survival curves
   - Survival probability estimation
   - Segment-based survival comparison
   - Log-rank tests for statistical significance

5. **Hazard Analysis**
   - Cox Proportional Hazards model
   - Hazard ratio calculation and visualization
   - Baseline hazard function estimation
   - Conditional churn probability analysis

6. **Parametric Survival Models**
   - Log-Normal distribution fitting
   - Weibull distribution fitting
   - Exponential distribution fitting
   - Model comparison using AIC

7. **Customer Lifetime Value Analysis**
   - Expected lifetime calculation
   - CLV estimation and segmentation
   - High-value customer identification
   - Financial impact analysis

8. **Cohort Analysis**
   - Tenure-based cohort creation
   - Cohort-specific churn patterns
   - Survival trends across cohorts

9. **Strategic Recommendations**
   - Data-driven retention strategies
   - High-risk segment identification
   - Targeted intervention timing
   - Value-maximizing approaches

![image](https://github.com/user-attachments/assets/690689bf-0ec5-47de-9e6f-96721b9aa779)

## 🔍 Key Insights

The analysis typically reveals several key insights that can drive business strategy:

- **Churn Timing Patterns**: Identification of high-risk periods in the customer lifecycle
- **Value Drivers**: Which services and features increase customer lifetime value
- **Risk Factors**: Customer attributes and behaviors that increase churn probability
- **Segment Performance**: Which customer segments have the highest/lowest retention
- **Intervention Windows**: Optimal timing for retention initiatives
- **Financial Impact**: Quantification of revenue impact from churn reduction

![image](https://github.com/user-attachments/assets/79af0d96-a261-4382-87e0-57c87e16cbdd)


## 📊 Visualization Examples

The script generates numerous visualizations to help understand churn patterns:

- Survival Curves by Customer Segment
- Hazard Ratios for Key Variables
- Feature Importance for Churn Prediction
- Customer Lifetime Value Distribution
- Cohort-Based Retention Analysis
- Parametric vs. Non-Parametric Survival Fits

## 🤝 Contributing

Contributions to improve the analysis are welcome! Please follow these steps:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Run tests to ensure functionality
5. Commit your changes (`git commit -m 'Add some amazing feature'`)
6. Push to the branch (`git push origin feature/amazing-feature`)
7. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📬 Contact

If you have any questions or feedback, please reach out:

- Project Link: [https://github.com/yourusername/telecom-churn-analysis](https://github.com/yourusername/telecom-churn-analysis)

---

### 📈 Survival Analysis Applications in Business

Survival analysis techniques used in this project have applications beyond telecom, including:

- **SaaS Customer Retention**: Analyzing subscription-based business models
- **Credit Risk**: Assessing time-to-default for loans
- **Insurance**: Policy lifetime and lapse risk analysis
- **Retail**: Customer lifetime value and repeat purchase behavior
- **Healthcare**: Treatment effectiveness and patient outcomes

The methods demonstrated here can be adapted to these and other domains with minimal modification.
