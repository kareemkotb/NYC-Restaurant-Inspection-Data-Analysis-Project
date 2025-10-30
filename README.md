# NYC-Restaurant-Inspection-Data-Analysis-Project

🏙️ Project Background

You are a Data Analyst at the New York City Department of Health (DOH). The department inspects restaurants citywide to ensure food safety and compliance with public health regulations. Each inspection results in a numerical score and a grade (A–C), influencing restaurant reputations and consumer trust.

The goal of this project is to analyze inspection data to uncover:

Which cuisines and boroughs have the most violations

The distribution of inspection grades

The most common violation types

Differences between critical and non-critical issues

Insights and recommendations are provided on the following key areas:

Borough & Cuisine Trends

Violation Patterns

Inspection Performance

Data Quality & Operational Efficiency

SQL scripts used in this project:

Data Cleaning & Preparation

Exploratory SQL Analysis

Tableau Dashboard

🗂️ Data Structure & Initial Checks

The dataset was sourced from NYC Open Data’s Restaurant Inspection Results database (~200K records).

Table Name	Description
restaurants	Restaurant information (name, cuisine, borough)
inspections	Inspection type, date, and score
violations	Violation codes and descriptions
boroughs	Mapping between borough codes and names

Entity Relationship Diagram (ERD)

restaurants (CAMIS) ---< inspections (CAMIS)
inspections (CAMIS) ---< violations (CAMIS)
boroughs (BORO_CODE) ---< restaurants (BORO_CODE)

📈 Executive Summary

Overview of Findings:

American cuisine restaurants had the highest number of violations (33,806), followed by Chinese (16,038) and Italian (13,971).

Bakery/Dessert and Beverage establishments had some of the lowest average inspection scores, indicating more consistent compliance.

Manhattan accounted for the largest number of inspections (95,732) and the highest number of critical violations (53,479).

The most frequent inspection type was Cycle Inspection / Initial Inspection (146,604), followed by Cycle Re-inspection (57,247).

About 50.9% of inspections had no grade (N), while 35.1% achieved an A.

🔍 Insights Deep Dive
Category 1: Borough & Cuisine Trends

Top cuisines by total violations:

American – 33,806

Chinese – 16,038

Italian – 13,971

Beverages – 12,940

Bakery/Desserts – 11,453

Cuisines with the lowest average scores (indicating better performance):

Specialty (21.91)

Bakery/Desserts (22.21)

Beverages (22.59)

American (22.76)

European (23.10)

American cuisine dominates inspection volume (61,834 inspections), followed by Chinese (27,007) and Italian (24,766).

Category 2: Borough Performance

Total inspections by borough:

Manhattan – 95,732

Brooklyn – 69,026

Queens – 64,455

Bronx – 24,030

Staten Island – 9,440

Boroughs with the highest number of critical violations:

Manhattan – 53,479

Brooklyn – 38,932

Queens – 36,742

Category 3: Inspection & Violation Patterns

Inspection Type Breakdown:

Cycle Inspection / Initial — 146,604

Cycle Re-inspection — 57,247

Pre-permit (Operational) / Initial — 37,340

Pre-permit (Operational) / Re-inspection — 10,464

Critical vs. Non-Critical Violations:

Critical: 147,805

Non-Critical: 114,878

Top 10 Most Frequent Violations:

Code	Description (Summary)	Count
10F	Food not protected from contamination	38,921
08A	Evidence of mice	26,254
06D	Improper temperature	18,000
02G	Food contact surface not clean	17,308
10B	Improper storage of utensils	17,142
06C	Food not refrigerated properly	16,733
04L	Vermin infestation	15,200
02B	Food contaminated	14,564
04N	Unclean surfaces	11,317
04A	Improper hand washing	7,746
Category 4: Grade Distribution
Grade	Count	Percentage
A	92,291	35.13%
B	17,433	6.64%
C	11,932	4.54%
N (Not Yet Graded)	133,677	50.89%
P (Pending)	838	0.32%
Z (Grade Pending Review)	6,512	2.48%

Over 35% of restaurants earn an “A”, while nearly half remain ungraded, often due to pending inspections or new openings.

💡 Recommendations

Based on these insights, the NYC DOH should consider:

Targeted Interventions: Focus compliance training on American, Chinese, and Italian restaurants with the highest violation counts.

Critical Violation Mitigation: Prioritize reducing food-temperature and pest-related violations, which make up over 40% of all critical issues.

Inspection Scheduling: Increase summer inspections when violations historically rise.

Public Transparency: Encourage posting of inspection results to incentivize better compliance.

Data Improvements: Standardize cuisine naming and inspection types to improve analysis accuracy.
