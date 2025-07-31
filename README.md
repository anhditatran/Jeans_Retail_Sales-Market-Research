## **Jeans_Retail_Sales-Market-Research**

### **1. Executive Summary**
This report presents a comprehensive analysis of the second-hand jeans retail market, based on a dataset of online sales listings. The primary objective was to identify the key metrics and dimensions driving brand performance, market trends, and pricing strategies. 

#### **Key Findings:**
* **Brand Performance is driven by a mix of Reputation and Price .**
  * **Levi's:** Dominates the market with the highest sales volume and the largest individual follower count at a moderate average price. However, it receives poor ratings, suggesting that for consumer retail, price is a primary driver of sales.
  * **Rick Owens:** Successfully commands the highest average price while maintaining a strong seller rating and high sales. This indicates that for premium brands, perceived quality and brand equity can justify a higher price point.
* **Geographic Concentration**
    * The market is heavily concentrated in three primary regions: **Asia, the US, and Europe**.
    * Asia is the top destination for shipping, indicating it is the primary online consumer base.
    * The US shows lower shipping volume, which may suggest a stronger consumer preference for in-store purchasing 
    * Individual brands appear to have distinct regional strengths that can be leveraged for more focused marketing efforts.
* **Price vs. Reputation**
    * A higher average price for a brand does **not** consistently correlate with a higher seller rating or more followers.
    * This suggests that factors beyond price, such as **brand reputation and seller service**, are critical drivers of customer satisfaction and loyalty.
* **Market & Product Trends**
    * A significant majority of listings are for **"gently used"** items, highlighting a robust market for high-quality, second-hand apparel.
    * Basic colors like **black and blue** remain highly popular.
    * For certain product categories, such as jeans, brand name appears to be a less significant purchasing factor for the average consumer.

### **2. Project Overview & Objectives**
* **Data Integrity:** To transform the raw dataset into a clean, reliable, and consistent resource for analysis.
* **Trend Identification:** To uncover and visualize underlying patterns in sales, pricing, brand popularity, and geographical distribution.
* **Insight Generation:** To derive actionable conclusions about market drivers that can inform strategic decision-making for buyers and sellers.
#### **2.2. Data Source**
The analysis is based on a static dataset of second-hand jeans listings aggregated from an online retail platform. The dataset includes fields such as `brand`, `price`, `condition`, `color`, `seller rating`, `follower count`, and `shipping options`.

### **3. Methodology**
#### **3.1. Tools and Libraries**
The project was executed in a Python environment, leveraging the following core data science libraries:
* **Data Manipulation & Computation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
#### **3.2. Data Preparation and Cleaning**
Before analysis, the data underwent a thorough cleaning and preparation phase:
1.  **Feature Engineering:** Structured, analyzable columns (`country_of_origin`, individual shipping costs per region) were engineered from unstructured text fields (`traits`, `shipping_options`). 
2.  **Handling Missing & Inconsistent Data:** Missing values in the `color` and `seller_rating` columns were imputed. Textual inconsistencies, such as typos and non-standard entries (e.g., "see photo"), were standardized to ensure data quality.
3.  **Outlier Management:** For the price distribution analysis, outliers were identified using the Interquartile Range (IQR) method to prevent extreme values from skewing the visualization of typical pricing.
#### **3.3. Exploratory Data Analysis (EDA)**
A combination of statistical summaries and visualizations was used to explore the data:
* **Distribution Analysis:** Histograms and pie charts were used to understand the frequency of key attributes like price, brand, and condition.
* **Comparative Analysis:** Dual-axis charts were employed to compare metrics with different scales, such as average brand price versus average seller rating.
* **Geographic Analysis:** A heatmap was generated to visualize the concentration of sellers by brand across different regions.

### **4. Conclusion & Future Work**
* **Predictive Modeling:** Developing a regression model to predict jean prices based on their features, which would provide a valuable tool for sellers.
* **Trend Analysis:** Incorporating time-series data to analyze how prices and brand popularity fluctuate seasonally or over time.
* **Interactive Dashboard:** Creating a web-based dashboard to allow for dynamic filtering and exploration of the data, making the insights more accessible to a non-technical audience.
