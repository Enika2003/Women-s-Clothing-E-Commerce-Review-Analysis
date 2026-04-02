# Women's Clothing E-Commerce Review Analysis

## Overview
This project analyzes customer reviews from a women's clothing e-commerce platform to identify patterns of customer satisfaction, dissatisfaction, and provide actionable insights for improving product performance.

## Business Problem
Analyze customer reviews to identify dissatisfaction factors and improve product performance across different departments, classes, and customer demographics.

## Key Metrics (KPIs)
- **Total Reviews**: Number of customer reviews analyzed
- **Average Rating**: Mean customer rating across all reviews
- **Recommendation Rate**: Percentage of customers who recommend the product
- **Negative Review Rate**: Percentage of reviews with rating ≤ 2
- **Average Positive Feedback Count**: Average helpful votes per review

## Analysis Components

### 1. Data Cleaning & Feature Engineering
- Removes duplicate records and missing values
- Creates age group categories (18-24, 25-34, 35-44, 45-54, 55+)
- Derives sentiment classification from ratings:
  - **Negative**: Rating ≤ 2
  - **Neutral**: Rating = 3
  - **Positive**: Rating ≥ 4
- Calculates review length metrics
- Standardizes recommendation indicators

### 2. Segmentation Analysis
- **By Department**: Average ratings across product departments
- **By Product Class**: Recommendation rates by clothing category
- **By Age Group**: Customer satisfaction and recommendation patterns across demographics

### 3. Text Analysis
- Extracts and analyzes keywords from negative reviews
- Identifies common complaint terms and pain points
- Uses custom stopwords filtering for meaningful insights

### 4. Visualizations
- Bar charts showing average ratings by department
- Recommendation rates by age group
- Positive feedback counts by sentiment

## Data Source
Women's Clothing E-Commerce Reviews Dataset  from Kaggle containing:
- Customer ratings and reviews
- Demographic information (age, department, class)
- Recommendation indicators
- Positive feedback counts

## Technologies Used
- **Python 3.x**
- **pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Matplotlib**: Data visualization
- **Regular Expressions**: Text processing


### Requirements
- Python 3.7+
- Jupyter Notebook or JupyterLab
- Required packages: pandas, numpy, matplotlib

### Installation
```bash
pip install pandas numpy matplotlib jupyter
```

### Running the Analysis
1. Ensure the raw data file `Womens Clothing E-Commerce Reviews.csv` is in `data/raw/` directory
2. From the notebook folder, open the notebook:
   ```bash
   jupyter notebook clothingtrend_analysis.ipynb
   ```
3. Run all cells to execute the analysis
4. Cleaned data will be saved to `data/cleaned/cleaned_fashion_data.csv`

## Key Findings
The analysis provides insights on:
- Which departments receive the lowest ratings
- Customer recommendation patterns by age group and product class
- Common complaints and issues identified in negative reviews
- Correlation between review sentiment and customer feedback

## Output
The cleaned and processed data is saved to `data/cleaned/cleaned_fashion_data.csv` for further analysis or integration with other tools.


## Author
Enika Krishnasamy Panjalingam

## License
MIT License

Copyright (c) 2026 Enika Krishnasamy Panjalingam

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
