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

#### **EDA**  
The exploratory data analysis revealed several key insights into Utah real estate trends:  

1. The **average property listing price** is approximately $797,000, though most properties are priced below $529,000.  
2. **Farm properties** tend to command significantly higher prices compared to other types, reflecting their size and utility.  
3. Properties are generally **newer**, with a construction peak around 2003, but the data includes a wide range of building years, from historic to upcoming builds.  
4. There is almost **no relationship between lot size and building size**, underscoring the diversity of property types in the market.  
5. **Garage spaces** are a common amenity but do not appear to strongly influence listing prices.  
6. **"For sale" properties** consistently fetch higher prices than "ready-to-build" lots, likely due to the immediate move-in potential.  

---

#### **Inferential Analysis**  
Our statistical exploration identified the following patterns impacting property values:  

1. **Bedroom Count**: More bedrooms correlate strongly with higher prices, as they typically provide more space and utility for buyers.  
2. **Year Built**: Homes constructed after 2000 are valued higher, likely due to their modern features and lower maintenance requirements.  
3. **Lot Size**: While larger lots generally cost more, their influence on overall price is minimal compared to other factors.  
4. **Garage Presence**: Surprisingly, the presence of a garage has a negligible impact on listing price.  
5. **Property Type**: Property types like single-family homes, condos, and townhouses have distinct pricing patterns, reflecting buyer preferences and lifestyle alignment.  

These findings are valuable for stakeholders to better understand which factors drive property pricing and prioritize features when buying or selling.  

---

#### **Machine Learning Insights**  
Predictive modeling provided the following results:  

| **Model**             | **R² Score** | **MAE**          | **MSE**             | **Key Insights**                                                                 |
|------------------------|--------------|-------------------|---------------------|----------------------------------------------------------------------------------|
| **K-Nearest Neighbors** | **0.9954**   | -                 | -                   | Outstanding performance, explaining 99.54% of the variance. Best suited for localized predictions. |
| **Gradient Boosting**   | 0.5643       | 306,382.10        | 1.83 trillion       | Moderate accuracy, significant error rates; requires further tuning for improvement. |
| **Random Forest**       | 0.5166       | 301,965.53        | 2.04 trillion       | Underperformed due to limited pattern capture; could benefit from better feature selection. |  

Among these, **KNN emerged as the top performer**, achieving near-perfect accuracy and explaining almost all data variance. Gradient Boosting and Random Forest models showed potential but require optimization to achieve comparable accuracy levels.  

---

#### **Conclusions**  
This analysis provides actionable insights for real estate stakeholders:  

- **Focus on Key Features**: Highlight attributes like bedroom count and recent renovations in listings to enhance perceived value.  
- **Utilize Predictive Models**: Deploy the KNN model for reliable property price predictions, enabling accurate market assessments.  
- **Timing Strategies**: Align property sales with seasonal peaks to maximize returns.  
- **Invest in Emerging Segments**: Townhouses and condos represent growth opportunities, particularly in Utah’s urban areas.  

---

#### **Recommendations**  
1. **Optimize Listings**: Emphasize property features that drive prices, such as size, age, and condition.  
2. **Enhance Model Accuracy**: Continue refining machine learning models with advanced techniques to improve predictive performance.  
3. **Create Tools for Real Estate Professionals**: Develop a dashboard integrating predictive models and insights for practical use.  

---

## Next Steps
1. **Advanced Modeling**: Explore deep learning techniques to further improve price prediction accuracy.  
2. **Geospatial Analysis**: Incorporate location-specific factors to refine market insights.  
3. **User-Friendly Tools**: Develop a dashboard for real estate professionals to access insights and predictive models.  

---

## For More Information

For more details, see the full analysis in the [project notebooks](https://github.com/quadrillionaiire/Utah-Real-Estate-Sales-Analysis/tree/main/notebooks) or review this[ presentation]((https://www.canva.com/design/DAGWc5fTdS0/woFwm899RyydP5aFscJM9Q/edit?utm_content=DAGWc5fTdS0&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton))
[https://www.canva.com/design/DAGWc5fTdS0/woFwm899RyydP5aFscJM9Q/edit?utm_content=DAGWc5fTdS0&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton](url)
---

## Repository Structure
- `data/`: Raw and cleaned datasets.  
- `notebooks/`: Jupyter Notebooks for EDA, inferential analysis, and machine learning.  
- `reports/`: Final Pipeline summary.
- `images/`: Key charts and graphs from the analysis.  
- `README.md`: Project overview and findings (this document).


