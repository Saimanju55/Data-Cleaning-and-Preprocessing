🏥 Task 1: Data Cleaning & Preprocessing

GitHub Repository: https://github.com/Saimanju55/Data-Cleaning-and-Preprocessing/edit/main/README.md

📋 PROJECT OVERVIEW

This internship task focuses on cleaning and preprocessing the Medical Appointment No Shows dataset using Python and Pandas.

The objective was to identify and resolve common data quality issues such as missing values, duplicate records, inconsistent formats, incorrect data types, and invalid entries.

🎯 TASK OBJECTIVE

Clean and transform a raw healthcare dataset into a structured, analysis-ready dataset suitable for reporting, visualization, and predictive modeling.

📊 DATASET USED

Name: Medical Appointment No Shows (Kaggle)
Format: CSV

Original Dataset:

Total Records: 110,527

Total Columns: 14

Missing Values: Checked

Duplicates: Checked

Final Dataset:

Cleaned Records: (after removing invalid values if any)

Columns: 15 (including engineered feature)

Data Completeness: 100%

🛠 CLEANING STEPS PERFORMED
1️⃣ Identify & Handle Missing Values ✅

Method Used:

.isnull()

.sum()

Result:

No significant missing values found / (Handled if present)

2️⃣ Remove Duplicate Records ✅

Method Used:
.drop_duplicates()

Result:

Duplicate rows removed (if any)

3️⃣ Standardize Column Names ✅

Transformation Applied:

Converted all column names to lowercase

Replaced spaces and hyphens with underscores

Example:

No-show → no_show

ScheduledDay → scheduledday

Benefit:
Improves readability and consistency in code.

4️⃣ Fix Date Format ✅

Columns Converted:

scheduledday

appointmentday

Method Used:
pd.to_datetime()

Impact:
Enabled time-based calculations and analysis.

5️⃣ Remove Invalid Age Values ✅

Issue Found:
Some records had negative age values.

Solution:
Filtered dataset to keep age ≥ 0.

Result:
Improved data validity.

6️⃣ Standardize Text Values ✅

Column Cleaned:

gender

Method Used:
.str.lower()

Ensured consistent formatting (e.g., Male / Female).

7️⃣ Convert Target Column to Binary ✅

Column: no_show

Transformation:

Yes → 1

No → 0

Why Important:
Machine learning models require numerical data.

8️⃣ Feature Engineering ✅
New Feature Created:

waiting_days
Calculated as:

appointmentday - scheduledday


Purpose:
Helps analyze whether longer waiting time increases no-show probability.

📊 RESULTS SUMMARY
══════════════════════════════════════════════
DATA QUALITY METRICS
══════════════════════════════════════════════

✔ Missing Values Handled
✔ Duplicate Records Removed
✔ Date Columns Standardized
✔ Invalid Ages Removed
✔ Column Names Standardized
✔ Target Variable Converted
✔ New Feature Engineered
✔ Dataset Ready for Analysis

🚀 HOW TO RUN
Install Requirements
pip install pandas numpy

Run the Script
python medical_data_cleaning.py

Expected Output

✔ Dataset loaded
✔ Missing values checked
✔ Duplicates removed
✔ Date formats converted
✔ Age validated
✔ Target column encoded
✔ Feature engineered
✔ Clean dataset saved

Output File:
cleaned_medical_no_show.csv

💡 KEY CONCEPTS APPLIED
Concept	Implementation	Why It Matters
Missing Value Handling	dropna()	Prevents biased analysis
Duplicate Removal	drop_duplicates()	Avoids repeated records
Date Conversion	pd.to_datetime()	Enables time analysis
Outlier Handling	Age filtering	Ensures data validity
Standardization	Lowercase formatting	Clean structure
Feature Engineering	waiting_days	Adds analytical value
📚 LEARNINGS & INSIGHTS
What I Learned

Importance of data validation before analysis

How to clean healthcare datasets

Why date conversion is crucial

Handling categorical and numerical data types

Feature engineering enhances dataset value

Clean data leads to reliable insights

📁 PROJECT STRUCTURE
medical-appointment-data-cleaning/
│
├── README.md
├── Medical_Appointment_No_Show.csv
├── cleaned_medical_no_show.csv
├── medical_data_cleaning.ipynb
└── (Optional) screenshots/

✅ TASK COMPLETION CHECKLIST

✔ Identified and handled missing values
✔ Removed duplicate records
✔ Standardized column names
✔ Converted date formats
✔ Fixed invalid age values
✔ Converted target column to numeric
✔ Created new analytical feature
✔ Documented all changes
✔ Uploaded to GitHub

🔗 REPOSITORY INFORMATION

Repository: https://github.com/Saimanju55/Data-Cleaning-and-Preprocessing/edit/main/README.md
Branch: main

📧 SUBMISSION SUMMARY

This project demonstrates practical skills in:

Data cleaning and preprocessing

Python & Pandas for data manipulation

Healthcare data handling

Feature engineering

Professional documentation

GitHub project management

The dataset is now clean, structured, and ready for visualization, reporting, or predictive modeling.
