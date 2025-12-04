# Hotel Bookings Data Cleaning

This project was to get familiar with the datacleaning in Python using the "Hotel Bookings" dataset from Kaggle.

## Project Steps

### 1. Load the Dataset
- Downloaded and extracted dataset from Kaggle
- Imported pandas
- Loaded `hotel_bookings.csv` 
- Looked at the dataset using `.head()`

### 2. Look at the Dataset
- Checked shape, column names, and data types (`df.info()`)
- Checked statistics with `.describe()`
- Found missing values with `df.isna().sum()`

### 3. Handle Duplicates
- Identified duplicate rows
- Removed duplicates and reset the index

### 4. Fix Invalids
- Created a new column `total_guests = adults + children + babies`
- Removed rows where total guests equaled zero 

### 5. Handle Missing Values
- Filled missing children values with 0
- Replaced missing country values with `Unknown`
- Filled missing `agent` and `company` values with 0 or 'None'

### 6. Convert and Create Date Columns
- Converted `reservation_status_date` to a datetime 
- Combined year, month, and day columns to create a full `arrival_date` column

### 7. Save Cleaned Dataset
- Exported the cleaned dataset to `data/hotel_bookings_cleaned.csv`

---

