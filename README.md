# Data_Analyst_Task1
Data Cleaning and Preprocessing for Elevate Data Analyst Interns

Task 1: Data Cleaning and Preprocessing
Internship: Elevate Data Analyst Internship (Alabs / Ministry of MSME)  
Project Objective
The objective of this task was to clean and prepare a raw dataset that contained null values, duplicates, and inconsistent formats to make it ready for analysis.  
Dataset
• Name: Netflix Movies and TV Shows  
• Source: Kaggle  
• Format: Excel (.xlsx)  
Tools Used
• Microsoft Excel: Used for data filtering, string manipulation, and formatting.  
Process and Changes Made
1. Standardized Column Headers: Renamed all headers to be uniform, lowercase, and without spaces (e.g., show_id, date_added, release_year).  
2. Handled Missing Values:
• Identified nulls in director, cast, and country using Excel filters.
• Filled missing categorical data with "Unknown" to maintain dataset integrity.
• Removed records with critical missing values in date_added and rating.
3. Removed Duplicate Records: Utilized Excel’s "Remove Duplicates" tool to ensure each show_id is unique.  
4. Standardized Date Formats:
• Challenge: Encountered inconsistent text-based dates with varying string lengths (1-digit vs. 2-digit days).
• Solution: Used a combination of TRIM, MID, FIND, and DATE functions to extract Year, Month, and Day components accurately.
• Result: Converted all records to a consistent dd-mm-yyyy format.
5. Fixed Data Types (Duration Column):
• Challenge: The duration column mixed two different units (minutes for movies and seasons for TV shows).
• Solution: Created a duration_unit column to preserve context, then stripped text suffixes ("min", "Season") to convert the values into integers (int).  
• Result: Enabled numerical analysis on durations across both types of content.  
Key Deliverables
• Cleaned Dataset: A structured file ready for analysis or modeling.  
• Summary of Changes: Documented steps for transparency and reproducibility.
