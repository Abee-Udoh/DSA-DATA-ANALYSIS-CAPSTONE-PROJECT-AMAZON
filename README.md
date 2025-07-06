# DSA-DATA-ANALYSIS-CAPSTONE-PROJECT-AMAZON
I developed a dynamic Excel Dashboard analyzing 1,465 Amazon product reviews, uncovering insights on ratings, pricing, discounts, and revenue. Using pivot tables, calculated columns, slicers, and visualizations, the data analysis aims to help sellers make smarter, data-driven decisions.

## Case Study 1: Amazon Product Review Analysis

### Project Overview
This Data Analysis project focuses on analyzing Amazon product and customer review data to generate actionable insights for e-commerce sellers. The core objective of this project was to empower sellers with the knowledge and tools to:
 - Improve product quality based on real customer feedback.
 - Refine marketing strategies using trends in reviews and ratings.
 - Boost customer engagement and satisfaction through informed decisions.
   
This Project aims to equips Amazon sellers with a strategic overview of how their products perform in the market, making it easier to spot opportunities, track customer sentiment, and make informed improvements.

### Dataset Description 
The dataset contains information scraped from Amazon product pages, including:
- Products details: name, category, price, discount, and ratings.
- Customer engagement: user reviews, titles, and content.
- Each row represents a unique product, with aggregated reviewer data stored as Amazon Case Study.xlsx.
- Dataset Size: 1,465 Rows | 16 Columns

### Tool Used: Microsoft Excel 
 
### Process: Data Cleaning, Preparation and Visualizations
- In the initial phase of the data cleaning and preparation, I performed the following actions:
  1. Apply the filter drop-down button to all header column. Go through each column to look for blanks and incorrect data. Replace the numeric blanks with 0.
  2. Remove duplicates from Product_Id. 
  3. Change the formatting of the columns where necessary i.e currency where necessary.
  4. Hide or delete unnecessary columns that you won't be needed to generate a result i.e img_link.
  5. For Category column, use delimiters in the Data tab to extract only the main category needed.
  6. Consistent and clean data with respect to data type, data format and values used.
  7. Create Pivot Tables to summarize and segment data efficiently.
  8. Calculated Columns to derive key performance indicators (e.g., Total potential revenue).
  9. Data Visualizations (Bar charts, tables, Pie chart, Scatter chart) to highlight trends in product ratings, discount behavior, pricing strategies, and review volume.
  10. Slicers and Filters for seamless interactivity and data exploration.

### Analysis Tasks & KPIs
Using Pivot Tables, Slicers, and Calculated Columns in Excel, the following questions were explored:
 1. What is the average discount   percentage by product category? 
 2. How many products are listed under each category?
 3. What is the total number of reviews per category? 
 4. Which products have the highest average ratings? 
 5. What is the average actual price vs the discounted price by category? 
 6. Which products have the highest number of reviews? 
 7. How many products have a discount of 50% or more? 
 8. What is the distribution of product ratings (e.g., how many products are rated 3.0, 4.0, etc.)? 
 9. What is the total potential revenue (actual_price × rating_count) by category?
10. What is the number of unique products per price range bucket (e.g., <₹200, ₹200–₹500, >₹500)? 
11. How does the rating relate to the level of discount? 
12. How many products have fewer than 1,000 reviews? 
13. Which categories have products with the highest discounts? 
14. Identify the top 5 products in terms of rating and number of reviews combined.

### Data Analysis 
Using Calculated columns, the following queries were used during the analysis:
 1. Average discount percentage by product category = (Actual Price - Discounted Price) / Actual Price * 100
 2. Discount of 50% or more =IF(Discount % >= 50, "Yes", "No")
 3. Total potential revenue by category =Actual Price * Rating Count
 4. Price bucket {=IF(Discounted Price < 200, "<$200", IF(Discounted Price <= 500, "$200–$500", ">$500")) }
 5. Rating + number of reviews combined = Average Rating + (Rating Count / Scaling Factor)(Choose a factor like 1000 to balance weight)
    
### Dashboard
https://github.com/Abee-Udoh/DSA-DATA-ANALYSIS-CAPSTONE-PROJECT-AMAZON/blob/main/Excel%20Dashboard.jpg

### Project insights
Some key takeaways from the analysis:
- Certain categories offer deeper discounts but lower ratings.
- A small group of products contributes the most to review volume and potential revenue.
- There's a slight inverse correlation between deep discounts and product ratings.
- Most products are priced between ₹200–₹500.

### Conclusion
 The Amazon Product Review Analysis in Excel uncovered key trends in product performance, pricing, and customer engagement. Insights such as the impact of discounts on ratings and concentration of reviews among top products provide actionable guidance for improving product strategy, marketing, and customer satisfaction.






