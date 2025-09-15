# iPhone Pricing & Value Analysis

## 📊 Project Overview
Analysis of iPhone pricing strategies on Flipkart, identifying value opportunities, pricing anomalies, and consumer rating patterns across 62 iPhone models.

## 🔍 Key Insights
- Discovered iPhone SE (64GB) offers best value.
- Identified 23% average price premium on certain color variants
- Found budget segment (₹30-50K) has highest average ratings (4.6/5)

## 🛠️ Technologies Used
- Python (Pandas, Plotly, NumPy)
- Data Cleaning & Feature Engineering
- Statistical Analysis
- PowerBI Dashboard

## 🚀 How to Run
1. Install: `pip install -r requirements.txt`
2. Run analysis: `jupyter notebook notebooks/Iphones sales Analysis.ipynb`
3. Explore dashboard: `dashboards/iphone_pricing_dashboard.pbix`

## Code Snippet: Example Visualization
```python
# Relationship between Sale Price and Number of Ratings
figure = px.scatter(data_frame=data,
                   x='Number Of Ratings',
                   y='Sale Price',
                   trendline='ols',
                   title='Relationship between Sale Price and Number of Ratings')
figure.show()
```


### 1. No. of ratings of highest-rated iPhones on Flipkart
Identified the highest-rated models. The iPhone 8 Plus (Gold) variant consistently received the highest ratings.

<img width="2400" height="1800" alt="iphone_vs_ratings" src="https://github.com/user-attachments/assets/c4db34d6-0b53-49fd-9db3-8bba19380287" />


### 2. Relationship between Sale Price and Number of Ratings
Discovered a strong inverse correlation – more affordable iPhones generate a significantly higher volume of customer ratings.

```python
figure = px.scatter(data_frame=data, x='Number Of Ratings', y='Sale Price', trendline='ols')
figure.show()
```
<img width="2200" height="1800" alt="relation_bw_saleprice_no_of_ratings" src="https://github.com/user-attachments/assets/d0dafb2d-7fd2-4e15-b15d-b59972d6a44d" />



### 3. Rating vs Price
- Value Perception Mapping: Visualizes whether premium pricing correlates with higher star ratings
- Customer Sentiment by Price Segment: Colors differentiate Budget, Mid-range, Premium, and Flagship devices
- Popularity Indicators: Bubble size represents number of ratings (market engagement)
- Product-Level Insights: Hover reveals specific iPhone models for detailed analysis

<img width="2400" height="1800" alt="Rating vs Price" src="https://github.com/user-attachments/assets/568f3c38-e5a8-4126-a400-92b49bdb8657" />

