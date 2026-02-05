# Retail-Sales-Transactions-Dashboard

#Exploratory Data Analysis (EDA)
#Dataset Overview
The dataset contains retail transaction records across multiple countries for the period 2009–2010.
Each record represents a single line item within an invoice.

# Key fields include:
- Invoice
- StockCode
- Description
- Quantity
- Price
- InvoiceDate
- CustomerID
- Country

# Data Cleaning & Preparation
Several preprocessing steps were performed before analysis:
- Combined multiple yearly datasets into a single table using append
- Removed or handled:
   - Null or missing values where appropriate
   - Invalid quantity values (e.g. negative or zero where not meaningful)
- Standardized data types:
   - InvoiceDate converted to Date/Time
   - Numerical fields (Price, Quantity) validated

- Created calculated measures using DAX:
    - Total Revenue
    - Total Quantity
    - Average Price
      
- Extracted time-based features:
    - Year  
    - Month (sorted chronologically using Month Number)

# Revenue Distribution
Initial exploration shows that:
  - Revenue is highly concentrated in a small number of countries
  - The United Kingdom is the dominant contributor to total revenue
  - Other European countries contribute smaller but consistent portions
This indicates a Pareto-like distribution, where a minority of countries drive the majority of revenue.

# Time-Based Trends
Exploring revenue over time revealed:
  - Clear seasonal patterns, with revenue peaking toward the end of the year (Q4)
  - Revenue trends are broadly consistent across years, though magnitude differs
  - Monthly analysis helps highlight demand cycles typical in retail businesses

# Sales Volume vs Pricing
EDA comparing quantity and price shows that:
  - High revenue does not always correlate with high sales volume
  - Some countries generate strong revenue with relatively lower quantities, suggesting higher average prices
  - This distinction highlights the importance of analyzing both volume and value, not revenue alone

