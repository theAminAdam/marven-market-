# marven-market
Project: Maven Market Data Analysis

Introduction:
The goal of the Maven Market project involves analysing data from various sources to derive insights and make informed business decisions. This data analysis project was conducted using Power BI, a powerful tool for visualizing and interpreting data. The goal of this project is to provide actionable insights to Maven Market stakeholders based on comprehensive data analysis.

---
## Part 1: Data Preparation:

Data was prepared using the following steps:

**Customer Table:**

  - Data from the MavenMarket_Customers csv file is imported and named as "Customers".
  - Ensured accurate data types, including whole numbers for customer_id, and text for customer_acct_num and customer_postal_code columns respectivel columns respectively.
  - Added a new column "Full_Name" by merging first_name and last_name.
  - Created "birth_year" column extracting the year from the "birthdate" and formatting it as text.
  - Created a conditional column "has_children" based on the presence of children.

**Products Table:**

  -  Data from the MavenMarket_Products csv file as "Products" is imported.
  -  Verified data types, including whole number for product_id, text for product_sku, and decimal numbers for product_retail_price and product_cost.
  -  Used statistics tools to find distinct product brands and names.
  -  Addded a calculated column "discount_price" at 90% of the original retail price, rounded to 2 digits.
  -  Calculated the average retail price by brand and name the new column "Avg Retail Price".
  -  Replaced "null" values with zeros in "recyclable" and "low-fat" columns.

**Stores Table:**

  -  Data from the MavenMarket_Stores csv file as "Stores" is imported,
  -  Ensured accurate data types, with whole numbers for store_id and region_id.
  -  Calculated column "full_address" was added by merging store_city, store_state, and store_country.
  -  Calculated column "area_code" was added by extracting characters before the dash in store_phone column.

**Other Tables:**

MavenMarket_Regions and MavenMarket_Calendar csv files were imported

  -  Data validation was carried out to ensure accurate data types and perform necessary data manipulations.

---
## Part 2: Building the Data Model:

  -  Tables in the MODEL view were arranged with lookup tables above data tables.
  -  Relationships between tables were established using valid primary and foreign keys.
  -  Date fields and relevant columns were formatted & categorized for improved analysis.

## Part 3: Implementing DAX Measures:

  -  DAX was used to add calculated columns and measures for various metrics such as transaction details, revenue, profit, returns, and more.
  -  Measures were formatted as appropriate for clear visualization.


## Part 4: Report Dashboard:

  -  Report layout was designed with relevant visuals, including matrices, KPI cards, maps, charts, and gauges.
  -  Bookmarks and notes were utilized to highlight key insights and trends.
  -  Interactive features like drill-down and filters were added for enhanced user experience.

A concise, informative, Dynamic Report Dashboard was Developed.

---
## Conclusion:

The **Maven Market** data analysis project leverages Power BI to transform raw data into actionable insights. By preparing the data, building a robust data model, implementing DAX measures, and constructing a comprehensive report, stakeholders can make informed decisions to optimize business operations and drive growth.
