# data_Analysit_project-telagana_vehicle_Registraion_jan-Telangana Vehicle Registration – Exploratory Data Analysis (January 2025)
Project Overview
This project involves exploratory data analysis (EDA) on Telangana's vehicle registration data for January 2025. The data is sourced from the Telangana State Transport Department and aims to uncover insights into vehicle types, fuel usage, registration trends, and data quality.

Objectives (Phase 1)
Understand the dataset structure, types, and quality.

Preprocess date fields and handle missing values.

Identify patterns in vehicle distribution and registration behavior.

Dataset Summary
Total Records: 343,137

Total Columns: 16 (registration number, fuel, manufacturer, model, etc.)

Most fields have no missing values except:

fuel: 3,778 missing and some invalid entries

regvalidfrom: 1,692 missing

reserve_no: 93% missing (as expected)

Key Findings
Vehicle Registration
Duplicated serial numbers (appear twice): 168,188 → 336,376 rows

Unique single serial numbers: 6,761

Total rows: 343,137

Data Cleaning
Missing registrationNo values were filled using reserve_no

One unusable row was removed

Converted regvalidfrom, regvalidto, fromDate, and toDate to datetime format

Feature Exploration
Manufacturer (makerName)
Most frequent:

ONDA MOTORCYCLE & SCOOTER (62,617)

MARUTI SUZUKI INDIA LTD (38,653)

BAJAJ AUTO LTD (35,937)

Vehicle Model (modelDesc)
Most common: ACTIVA-DLX BSVI-PH2 (11,560 records)

Highly skewed distribution with thousands of rare models

Body Type
Most common body types:

Solo: 181,842

Sedan: 43,885

Open: 36,500

Hatchback: 35,328

Saloon: 13,386

Total unique body types: 39

Fuel Type
Most common:

PETROL: 231,422

DIESEL: 81,638

BATTERY: 12,709

Invalid entries: -1, 0, lowercase 'petrol'

Fuel type imputed based on cc, cylinder, hp, seatCapacity

Seat Capacity
Most common values:

2 seats: 191,919

5 seats: 85,155

1 seat: 20,745

7 seats: 13,164

4 seats: 12,523

Rare values include 61 seats and 38 seats (2 records each)

Engine Specifications
Cylinder:

1 cylinder: 185,720 (mostly two-wheelers)

4 cylinders: 88,853

3 cylinders: 40,469

6, 8, 10, 12 cylinders are rare

CC (engine displacement):

Common values: 124.0 cc, 97.0 cc, 1197.0 cc

Total unique CC values: 588

Horsepower:

Total unique values: 1,055

Top values include: 7.91, 7.74, 8.58, 88.51, 8.19

Office Code (officeCd)
Total unique RTA/UNIT branches: 56

No missing values

Standardized prefixes ("RTA", "UNIT") for region classification

Final Summary
The dataset is highly skewed toward a few manufacturers, models, and fuel types.

Clean, rich vehicle registration data suitable for visualization, modeling, and trend analysis.

This EDA sets the foundation for further machine learning, clustering, or predictive analysis in upcoming phases.

Author
Name: Doddipatla Vishnu Durga
Background: B.Tech in Computer Science and Engineering (2025)
LinkedIn: linkedin.com/in/vishnu-durga-ddldipatha7-6h3l3d2b
GitHub: github.com/Vishnu8o7

