# Zomato Bangalore Restaurants Case Study  

## Overview  
This dataset provides information about restaurants in Bangalore listed on Zomato. The data includes various categories of restaurants such as Buffets, Cafes, Delivery services, Desserts, Dine-out options, Drinks & nightlife, and Pubs & bars. It aims to help users identify the best restaurants based on their preferences and requirements.  

## About Zomato  
Zomato is an Indian multinational restaurant aggregator and food delivery company, founded by **Deepinder Goyal** and **Pankaj Chaddah** in 2008. The platform provides:  
- Information about restaurants.  
- Menus and user reviews.  
- Food delivery options from partner restaurants in selected cities.  

## Dataset Information  
The dataset focuses on restaurants in Bangalore working with Zomato and was collected in two phases via web scraping.  

## Data Columns  
The dataset includes the following columns:  

| **Column Name**             | **Description**                                                                            |  
|------------------------------|--------------------------------------------------------------------------------------------|  
| `url`                        | The URL of the restaurant's Zomato page.                                                  |  
| `address`                    | The address of the restaurant.                                                            |  
| `name`                       | Name of the restaurant.                                                                   |  
| `online_order`               | Indicates if online ordering is available (Yes/No).                                       |  
| `book_table`                 | Indicates if table booking is available (Yes/No).                                         |  
| `rate`                       | User rating of the restaurant.                                                            |  
| `votes`                      | Total number of votes received for the restaurant.                                        |  
| `phone`                      | Contact number of the restaurant.                                                         |  
| `location`                   | Neighborhood or area where the restaurant is located.                                     |  
| `rest_type`                  | Type of restaurant (e.g., Casual Dining, Café, Pub).                                      |  
| `dish_liked`                 | Most liked dishes mentioned by users.                                                     |  
| `cuisines`                   | Types of cuisines offered by the restaurant.                                              |  
| `approx_cost(for two people)`| Approximate cost for two people.                                                           |  
| `reviews_list`               | List of reviews for the restaurant.                                                       |  
| `menu_item`                  | List of menu items available.                                                             |  
| `listed_in(type)`            | Category of the restaurant (e.g., Buffet, Café, Delivery).                                |  
| `listed_in(city)`            | City or locality in Bangalore where the restaurant is listed.                             |  
  

## Data Cleaning Process  
To ensure the dataset is clean, consistent, and ready for analysis, the following steps were undertaken:  

1. **Deleting Redundant Columns**:  
   Removed unnecessary columns that do not provide significant value for analysis or are irrelevant.  

2. **Renaming Columns**:  
   Updated column names to make them more descriptive and easier to understand.  

3. **Dropping Duplicates**:  
   Identified and removed duplicate rows to ensure data integrity.  

4. **Cleaning Individual Columns**:  
   - Standardized text data (e.g., removing extra spaces, converting to lowercase).  
   - Corrected spelling errors in categorical values.  

5. **Handling Missing Values**:  
   - Removed rows with NaN values to maintain consistency.  
   - Where appropriate, fill missing values with default or calculated values.  

6. **Additional Transformations**:  
   - Converted data types (e.g., from string to numeric) for analysis compatibility.  
   - Extracted useful information from combined columns.  
   - Added calculated fields for deeper insights (e.g., average cost per person).  
