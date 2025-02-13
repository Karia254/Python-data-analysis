# Airbnb Listings Data Cleaning, EDA Project: New York 2024


**Project Overview**

This project focuses on data cleaning, transformation and exploratory data analysis (EDA) of Airbnb listings in New York for 2024. The goal is to uncover trends, patterns and insights into the rental market, helping to understand pricing, availability, and other key factors influencing Airbnb listings

---
**Project Objectives**
1. Analyze room types, pricing, and availability across different neighborhoods to identify market trends.
2. Detect and handle potential outliers in pricing to improve data quality.
3. Perform univariate analysis on price and availability distribution across different neighborhoods.
4. Examine the relationship between price and neighborhood to understand location-based pricing variations.
5. Analyze the correlation between price and the number of reviews to explore how customer feedback influences pricing

---
**Data Set**

The AirBnB Listings Dataset has 20,765 rows and 22 columns including the following features;
1. **id**: Unique identifier for each listing
2. **name**: Title of the Airbnb listing
3. **host_name**: Name of the host
4. **neighborhood_group**: Group (borough) where the listing is located
5. **latitude/longitude**: Geolocation of listings
6. **price**: Nightly rental price
7. **room_type**: Type of accommodation (e.g., entire home, private room)
8. **reviews_per_month**: Average monthly reviews for the listing
9. **availability_365**: Number of available days in the year
    
---
**Steps**

**Data Cleaning and Transformation**

1. **Handle missing data**: Filled or removed null values in the price, neighborhood, and beds columns.
2. **Remove duplicates**: Ensured each listing is unique to prevent redundancy.
3. **Fix data types**: Converted last_review to a datetime object for accurate analysis.
4. **Remove outliers**: Capped listings with prices above $2,000 to prevent skewed visualizations.
5. **Add a new column for price per bed**: Calculated price per bed for better price comparisons.
   
 ---  
 **Exploratory Data Analysis**
 
1. Analyzed price variations using a histogram: Most listings were priced between $50 and $300.
2. Calculated the average price per neighborhood:
  . Manhattan had the highest average price at $208.21.
  . Bronx had the lowest average price at $107.99.
3.  Computed the average price per bed for each neighborhood to understand price variations relative to accommodation size.
4. Visualized the average price for different room types per neighborhood using a bar plot.
5. Analyzed the relationship between price and the number of reviews, visualizing it with a scatter plot to identify trends.


---
   **Key Insights**
1. Manhattan has the most expensive listings, followed by Brooklyn.
2. Entire homes/apartments cost significantly more than private or shared rooms.
3. Entire homes/apartments are the most common type of listing, but private rooms offer budget-friendly options.
4. Listings with high availability tend to have lower prices and more reviews, likely due to a better guest experience.
5. There are very few listings priced at $10,000 and above; most prices are below $2,000, indicating the need to filter out such extreme values.
