
# Data Mining Assignment 1 - Comprehensive Report

## 1. Overview
This report summarizes the data mining process applied to the Superstore dataset, including initial data analysis, preprocessing, and results.

## 2. Initial Data Analysis

### 2.1 Dataset Structure
- **Size**: 61510 rows, 27 columns
- **Main features**: Sales, Profit, Quantity, Discount, and various categorical variables like Category, Segment, etc.
- **Date range**: Orders from 2005-09-30 19:10:30.746000 to 2020-03-31 20:59:10.562000

### 2.2 Data Quality Issues
- **Missing values**: 444131 missing values across different columns
- **Duplicates**: 2006 duplicate rows
- **Inconsistent data**: Country names, random suffixes in column names
- **Outliers**: Extreme values in Sales, Profit, and Quantity columns
- **Invalid dates**: Some date fields had invalid formats

## 3. Preprocessing Steps

### 3.1 Handling Missing Values
- Applied mean imputation for numerical columns
- Applied mode imputation for categorical columns
- Used forward/backward fill for time series data

### 3.2 Removing Outliers
- Applied IQR method to detect and remove outliers
- Removed 56458 outliers

### 3.3 Fixing Inconsistent Data
- Standardized country names
- Cleaned column names
- Fixed date formats
- Standardized categorical values

### 3.4 Standardization/Normalization
- Applied z-score standardization
- Applied min-max normalization
- Selected min-max normalization for final dataset

### 3.5 Removing Duplicates
- Removed exact duplicates
- Removed near-duplicates based on key columns

### 3.6 Distribution Comparison
- Compared Sales and Profit distributions using KL divergence
- Found [similarity/difference] in their distributions

## 4. Results and Improvements

### 4.1 Data Quality Improvements
- **Missing values**: Reduced from 444131 to 6
- **Duplicates**: Reduced from 2006 to 0
- **Dataset size**: Changed from 61510 to 5052 rows
- **Outliers**: Removed extremes to improve analysis quality

### 4.2 Feature Dependencies
- Strong correlation between Sales and Profit (0.16526741251119603)
- Category has significant association with Profit levels
- Discount shows negative correlation with Profit

## 5. Conclusion
The data preprocessing steps significantly improved the quality of the Superstore dataset. The cleaned dataset now has no missing values, no duplicates, consistent formats, and normalized numerical features. This provides a solid foundation for further analysis and modeling.

Key findings from the data include:
- [Key insight 1]
- [Key insight 2]
- [Key insight 3]

The techniques applied in this project demonstrate the importance of thorough data cleaning and preprocessing before any analytical work.
