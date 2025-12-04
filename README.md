# Retail Price Optimization Engine

An end-to-end machine learning system for dynamic retail pricing optimization that analyzes competitor data, customer behavior, and market trends to maximize revenue.

## Project Overview

This project develops a data-driven pricing recommendation system for retail businesses, leveraging machine learning to predict demand and identify optimal price points. The system achieved a projected 129% revenue increase through intelligent pricing strategies.

## Key Results

- Model Accuracy: R² = 0.590 (59% variance explained)
- Revenue Impact: +129.4% projected increase
- Additional Revenue: $1,098 from optimized pricing
- Products Analyzed: 5+ product categories
- Time Period: 18+ months of historical data

## Technologies Used

- Python 3.x
- Pandas for data manipulation and analysis
- NumPy for numerical computations
- Scikit-learn for machine learning models (Random Forest, Gradient Boosting)
- Matplotlib and Seaborn for data visualization
- Jupyter Notebook as development environment

## Project Features

### Exploratory Data Analysis
The project begins with comprehensive data exploration to understand sales patterns, revenue trends across different product categories, and customer purchasing behavior over time.

### Price Elasticity Analysis
I analyzed how sensitive customer demand is to price changes by calculating price elasticity coefficients. This helps identify which products can support price increases and which require more competitive pricing.

### Competitor Analysis
The system tracks pricing across three major competitors, providing insights into competitive positioning and helping identify opportunities where strategic pricing adjustments could capture more market share.

### Demand Forecasting Model
Using ensemble machine learning methods, I built predictive models that forecast product demand based on price, competitor actions, seasonality, and other factors. After testing multiple approaches, Gradient Boosting provided the best performance with an R² score of 0.590.

### Dynamic Pricing Recommendations
The core feature simulates different pricing scenarios for each product, identifying the optimal price point that maximizes revenue while considering competitive dynamics and demand elasticity.

## Technical Approach

The project follows a structured data science workflow:

1. **Data Collection and Preparation**: Cleaned and preprocessed 18+ months of retail transaction data including sales volumes, pricing, and competitor information
2. **Feature Engineering**: Created 25+ derived features including price ratios relative to competitors, lagged sales variables, temporal indicators, and competitive positioning metrics
3. **Model Development**: Trained and evaluated multiple machine learning algorithms, ultimately selecting Gradient Boosting for its superior performance
4. **Optimization Engine**: Developed a price simulation system that tests various price points to identify revenue-maximizing strategies
5. **Business Recommendations**: Generated concrete pricing recommendations with projected revenue impacts for business stakeholders

## Project Structure
```
retail-price-optimization/
├── price_optimization_analysis.ipynb   # Main analysis notebook
├── README.md                            # Project documentation
├── requirements.txt                     # Python dependencies
└── data/
    └── retail_price.csv                # Dataset
```

## Getting Started

To run this project locally:
```bash
# Clone the repository
git clone https://github.com/suddhasheel333/retail-price-optimization.git

# Navigate to project directory
cd retail-price-optimization

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook price_optimization_analysis.ipynb
```

## Dataset Information

The dataset is included in this repository at `data/retail_price.csv`.

**Dataset characteristics:**
- Size: 67 KB
- Records: 5,000+ transactions
- Features: 30+ variables
- Time span: May 2017 through August 2018

**Key variables include:**
- Product identifiers and category information
- Sales metrics including quantity sold and revenue
- Our pricing and freight costs
- Competitor pricing from three major competitors
- Temporal indicators such as dates, holidays, and weekends
- Product attributes like weight, photos, and descriptions

## Key Insights and Findings

Through this analysis, several important patterns emerged:

- Customer demand for these products is elastic, meaning customers are price-sensitive and respond significantly to price changes
- Competitive positioning matters significantly. When priced below competitors, sales volume increases substantially
- Seasonal patterns play an important role, with certain months showing consistently higher demand
- Including lagged sales data improved model accuracy by 49% over the baseline approach
- The revenue-maximizing price point often differs from the profit-maximizing price, requiring strategic decisions about business objectives

## Business Value

This pricing optimization system provides several practical benefits for retail businesses:

- Enables data-driven pricing decisions rather than intuition-based approaches
- Allows quick response to competitor price changes
- Helps maximize revenue while maintaining competitive market positioning
- Quantifies customer price sensitivity for better strategic planning
- Supports inventory planning through improved demand forecasting

## Model Performance Summary

| Metric | Value |
|--------|-------|
| R² Score | 0.590 |
| Model Type | Gradient Boosting Regressor |
| Performance Improvement | +49% over baseline Random Forest |
| Training Approach | 80/20 train-test split with cross-validation |

## Future Development

Several enhancements could extend this work:

- Build an interactive dashboard using Streamlit for real-time pricing recommendations
- Implement A/B testing framework to validate pricing changes in production
- Integrate with inventory management systems for holistic supply chain optimization
- Develop customer segment-specific pricing strategies
- Add automated monitoring and alerting for significant competitor price changes
- Incorporate time-series forecasting methods like ARIMA or Prophet for improved temporal predictions

## About This Project

This project was developed as part of my data science portfolio to demonstrate practical machine learning applications in retail analytics. The focus was on creating an end-to-end solution that not only achieves good predictive performance but also translates technical results into clear business value.

## Author

Suddhasheel  
GitHub: [@suddhasheel333](https://github.com/suddhasheel333)

