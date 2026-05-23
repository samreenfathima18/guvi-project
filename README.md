Uber Eats Bangalore Restaurant Intelligence & Decision Support Systems
Project Overview:
This project is a Decision Support System (DSS) designed to analyze the Uber Eats restaurant ecosystem in Bangalore. Unlike traditional dashboards that rely on charts, this system mirrors internal corporate analytics tools where stakeholders require precise, tabular data to drive strategy.The system uses Python for ETL, MySQL/SQLite for the analytical engine, and Streamlit to deliver a clean, spreadsheet-style interface for business users.

Tech Stack & SkillsLanguage: Python 3.xData Manipulation: Pandas, 
NumPyDatabase: MySQL / SQLite (Relational Modeling & Complex Querying)
Web Framework: Streamlit (UI/UX for Data Tables)
Core Skills: ETL Pipelines, Data Cleaning, Statistical Segmentation, SQL Feature Engineering.

 Business Logic & SQL Insights:
 
 The application is divided into two primary modules:
 
 1. Dynamic Dashboard: A filter-driven interface where users can query the database in real-time by location, cuisine, or price segment. All logic is handled via SQL WHERE and LIKE clauses to ensure high performance.
2. Strategic Q&A (Top 10 Business Insights): The system answers critical questions using advanced SQL (Window Functions, CASE statements, and Aggregations):
 Location Intelligence: Identifying over-saturated vs. high-performing zones.
 Feature ROI: Analyzing if Online Ordering and Table Booking actually correlate with   higher Ratings.
 Pricing Strategy: Determining the "Sweet Spot" cost for maximum customer satisfaction.
 Niche Discovery: Finding cuisines with low supply but high ratings

Data Pipeline Approach Extraction:
Load raw restaurant data (CSV) and transactional orders (JSON).
Transformation (Pandas):
Normalization: Converting ratings (e.g., "4.1/5") to float.
Cleaning: Handling nulls in approx_cost and removing duplicates.
Feature Engineering: Creating Price_Segment (Budget, Mid, Premium) using statistical quantiles.
Loading: Migrating cleaned DataFrames into a Relational Database using SQLITE3.
Analysis: Executing cursor-based SQL queries to populate Streamlit st.dataframe() components.

Key Results Mid-tier Success:
 Analysis revealed that mid-priced restaurants consistently hold the highest average ratings compared to budget or ultra-premium spots.
Feature Impact: Restaurants offering both Online Ordering and Table Booking see a ~15% lift in average rating scores.
Expansion Strategy: Identified 3 specific neighborhoods in Bangalore with high order volume but "Below Average" food ratings, signaling a prime opportunity for high-quality partner onboarding.
