# DECODELABINTERNSHIP
This is where I document my internship task at DecodeLab
## TASK 1
## Project Title: Data Cleaning and Preparation
## Dataset Description: 
The dataset is an e-commerce orders with 1,200 rows and 14 columns, covering orders from 1 January 2023 to 30 June 2025.
## Goals: 
- Clean a raw dataset by handling missing values, duplicates, and incorrect data.
## Requirements:
• Identify missing or null values
• Remove duplicates
• Correct data formats (dates,
numbers, text)
### Skills:
Data cleaning and data preparation using Excel

# Data Cleaning
- I kept the original data untouched in a Raw_Data sheet and did all my work in a separate Cleaned_Data sheet.
- I counted rows and columns, then checked the unique values in every text column to look for typos and inconsistent spellings.
- # Missing Values:
  I found out that there are missing values in the CouponCode Column. I use the formula =COUNTBLANK to count all missing values. There was 309 missing values from a data set of 1200.
 - ### Decision:
 I replaced the blanks with "No Coupon" instead of filling them with the most common coupon. A blank here most likely means the customer didn't use a coupon, so filling it with an existing code would have invented coupon usage that never happened.

  - ### Formula:
    I selected the blank cells with Go To Special > Blanks, typed No Coupon and pressed Ctrl + Enter. Afterwards, COUNTBLANK returned 0.
- ## Duplicates
  - Removed duplicates on all columns found 0 duplicate rows.
  - Checking OrderID and TrackingNumber on their own also found 0 duplicates.
  - 11 CustomerIDs appear twice, but each has different orders, dates and products. These are repeat customers, not duplicates, so I kept them.
  - ### Format Data
    A dataset were corrected to the right data format.
    - Dates: all stored as real dates.
  ### Lesson
   - A blank cell doesn't always mean something is missing. Sometimes it means "no". Understanding what the column represents decides how you handle it.
   - Not every repeated ID is a duplicate. Removing the 11 repeat customers would have deleted real orders.
   - Writing down every decision and the reason for it matters as much as the cleaning itself.
    
