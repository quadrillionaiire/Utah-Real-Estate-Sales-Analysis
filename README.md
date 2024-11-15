# Utah Real Estate Sales Analysis and Predictive Modeling

## Overview
This project analyzes a dataset of real estate listings in Utah to uncover market trends, pricing dynamics, and factors influencing sales prices. By leveraging statistical methods and machine learning models, the analysis aims to provide actionable insights for property investors and real estate professionals. Key goals include understanding the drivers of property value, identifying trends in sales, and building predictive models to estimate property prices.

The findings will empower stakeholders to make informed decisions, optimize investments, and enhance market strategies.

---

## Business Problem
The Utah real estate market is dynamic and competitive, with numerous factors influencing property values. Professionals in the industry face challenges such as determining fair property prices, identifying market trends, and predicting the value of prospective investments. This analysis addresses three critical questions:

1. What property features (e.g., type, size, location) most influence listing prices?  
2. How do real estate prices vary over time and across property types?  
3. Can predictive models accurately estimate property prices based on listing characteristics?

By answering these questions, the project provides real estate stakeholders with tools to navigate the Utah market effectively.

---

## Data Understanding
The dataset includes 4,440 unique real estate listings sourced ethically via Apify's API and Realtor.com. Key attributes include:

- **Property Type**: Single-family homes, condos, townhouses, land, etc.  
- **Size Features**: Bedrooms, bathrooms, square footage, and lot size.  
- **Pricing**: Listing price and sales history.  
- **Additional Features**: Garage spaces and year built.  
- **Temporal Information**: Date of last sale.

The comprehensive nature of the dataset makes it suitable for exploratory analysis, inferential statistics, and machine learning.

---

## Data Preparation
The dataset underwent the following processing steps:

- **Data Cleaning**: Addressed missing values and standardized property types (e.g., grouped all condo-related categories under "Condo").  
- **Feature Engineering**: Created new columns such as property age, and sales trends over time.  
- **Outlier Detection**: Identified and excluded extreme outliers to maintain analysis integrity using IQR.  
- **Train-Test Split**: Split data into training and testing sets for machine learning.  

---

## Measure of Success
The primary measure of success for this project is the accuracy of predictive models. Each model aims to achieve a minimum of **75% accuracy** in estimating listing prices, ensuring actionable insights for stakeholders.

---

## Analysis & Results

### Key Market Insights:
1. **Top Factors Influencing Price**:  
   - Larger properties (in square footage and lot size) command higher prices.  
   - Properties with more bedrooms and bathrooms have a positive correlation with price, though diminishing returns are observed beyond 4 bedrooms.  

2. **Temporal Trends**:  
   - Average property prices have steadily increased from 2015 to 2023.  

3. **Property Type Analysis**:  
   - Single-family homes and condos are the most common property types, with farms generally commanding higher prices.  
   - Townhouses represent a growing segment, offering a balance of affordability and features.  

### Machine Learning Insights:
Predictive modeling revealed the following:  

- **K Nearest Neighbors**:  
  Achieved 99% accuracy with features like square footage, property age, and lot size as top predictors.  

- **Gradient Boosting**:  
  While useful, this model requires more tuning to improve performance.

- **Random Forest**:  
  Its performance could be enhanced by increasing tree depth or using advanced feature engineering.

---

## Conclusions
This analysis highlights critical insights for real estate stakeholders:  

1. **Focus on Size and Location**: Larger properties in desirable locations are key drivers of higher prices.  
2. **Timing Matters**: Listing properties during peak summer months can maximize sales prices.  
3. **Invest in Growing Segments**: Townhouses and condos represent emerging opportunities in Utah's real estate market.

---

## Recommendations
1. **Optimize Property Listings**: Highlight features like size, garage spaces, and recent renovations to justify pricing.  
2. **Leverage Predictive Tools**: Use the developed models to estimate fair market prices and identify undervalued properties.  
3. **Market Timing Strategy**: Align sales efforts with seasonal price peaks to capitalize on demand.  

---

## Next Steps
1. **Advanced Modeling**: Explore deep learning techniques to further improve price prediction accuracy.  
2. **Geospatial Analysis**: Incorporate location-specific factors to refine market insights.  
3. **User-Friendly Tools**: Develop a dashboard for real estate professionals to access insights and predictive models.  

---

## Repository Structure
- `data/`: Raw and cleaned datasets.  
- `notebooks/`: Jupyter Notebooks for EDA, inferential analysis, and machine learning.  
- `models/`: Trained machine learning models and evaluation metrics.  
- `visualizations/`: Key charts and graphs from the analysis.  
- `README.md`: Project overview and findings (this document).  

For more details, see the full analysis in the project notebooks.
