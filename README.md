This repository contains the cleaned dataset prepared by Jagadeshwari P
The original dataset was taken from Kaggle, and this cleaned version is ready for analysis and modeling
Cleaning Steps Performed

1.Column Renaming

All column names converted to lowercase and spaces replaced with underscores.

Example: AppointmentDay → appointmentday, Handcap → handicap.

2.Datetime Conversion

Converted scheduledday and appointmentday to proper datetime format.

3.Target Variable Encoding

No-show column converted to numeric:

No → 0

Yes → 1

4.Data Type Fixes

patientid converted to string (to avoid scientific notation).

5.Data Cleaning

Removed duplicates → 0 rows removed.
Cleaned Dataset Info

Total rows (after cleaning): 110,526

Total columns: 14

File name: noshowappointments_cleaned.csv

Removed invalid ages (< 0) → 1 row removed.

Checked for missing values → 0 found.
How to Use

step 1:Download the dataset:

noshowappointments_cleaned.csv


step 2:Load in Python:

import pandas as pd
df = pd.read_csv("noshowappointments_cleaned.csv")
print(df.head())
