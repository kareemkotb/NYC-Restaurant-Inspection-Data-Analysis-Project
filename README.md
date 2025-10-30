# NYC-Restaurant-Inspection-Data-Analysis-Project

## 🏙️ Project Background  

At the **New York City Department of Health (DOH)**.  
The department inspects restaurants citywide to ensure food safety and compliance with public health regulations.  
Each inspection results in a **numerical score** and a **grade (A–C)**, which affect restaurant reputations and consumer trust.  

This project analyzes NYC restaurant inspection data to uncover:  
- Which cuisines and boroughs have the most violations  
- The distribution of inspection grades  
- The most common violation types  
- Differences between **critical** and **non-critical** issues  

**Insights and recommendations** are provided on the following key areas:  
- Borough & Cuisine Trends  
- Violation Patterns  
- Inspection Performance  
- Data Quality & Operational Efficiency  

---

## 🗂️ Data Structure & Initial Checks  

The dataset was sourced from **NYC Open Data – Restaurant Inspection Results** (~200,000 records).  

| Table Name | Description |
|-------------|-------------|
| `restaurants` | Restaurant information (name, cuisine, borough) |
| `inspections` | Inspection type, date, and score |
| `violations` | Violation codes and descriptions |
| `boroughs` | Mapping between borough codes and names |

**Entity Relationship Diagram (ERD):**  


---

## 📈 Executive Summary  

**Key Findings:**  
- **American cuisine** had the most violations (**33,806**), followed by **Chinese (16,038)** and **Italian (13,971)**.  
- **Bakery/Desserts** and **Beverage** shops had the **lowest average inspection scores**, indicating better compliance.  
- **Manhattan** recorded the **most inspections (95,732)** and **most critical violations (53,479)**.  
- The majority of inspections (**50.9%**) were **ungraded (N)**, while **35.1%** achieved an **A**.  
- The most frequent inspection type was **Cycle Inspection / Initial Inspection** (146,604).  

![Dashboard Snapshot](#)

---

## 🔍 Insights Deep Dive  

### 🧆 Category 1: Borough & Cuisine Trends  

**Top 5 Cuisines by Violations:**  
| Cuisine | Violations |
|----------|-------------|
| American | 33,806 |
| Chinese | 16,038 |
| Italian | 13,971 |
| Beverages | 12,940 |
| Bakery/Desserts | 11,453 |

**Cuisines with Lowest Average Scores (Better Performance):**  
| Cuisine | Avg. Score |
|----------|-------------|
| Specialty | 21.91 |
| Bakery/Desserts | 22.21 |
| Beverages | 22.59 |
| American | 22.76 |
| European | 23.10 |

**Inspection Volume by Cuisine:**  
| Cuisine | Inspections |
|----------|--------------|
| American | 61,834 |
| Chinese | 27,007 |
| Italian | 24,766 |
| Beverages | 23,808 |
| Bakery/Desserts | 21,131 |

---

### 🏙️ Category 2: Borough Performance  

**Total Inspections by Borough:**  
| Borough | Inspections |
|----------|--------------|
| Manhattan | 95,732 |
| Brooklyn | 69,026 |
| Queens | 64,455 |
| Bronx | 24,030 |
| Staten Island | 9,440 |

**Critical Violations by Borough:**  
| Borough | Critical Violations |
|----------|---------------------|
| Manhattan | 53,479 |
| Brooklyn | 38,932 |
| Queens | 36,742 |
| Bronx | 13,299 |
| Staten Island | 5,353 |

---

### 🧾 Category 3: Inspection & Violation Patterns  

**Top Inspection Types:**  
| Inspection Type | Count |
|------------------|-------|
| Cycle Inspection / Initial | 146,604 |
| Cycle Inspection / Re-inspection | 57,247 |
| Pre-permit (Operational) / Initial | 37,340 |
| Pre-permit (Operational) / Re-inspection | 10,464 |
| Pre-permit (Non-operational) / Initial | 3,657 |

**Critical vs. Non-Critical Violations:**  
| Type | Count |
|-------|-------|
| Critical | 147,805 |
| Non-Critical | 114,878 |

**Top 10 Most Frequent Violation Codes:**  
| Code | Description (Summary) | Count |
|------|------------------------|-------|
| 10F | Food not protected from contamination | 38,921 |
| 08A | Evidence of mice | 26,254 |
| 06D | Improper food temperature | 18,000 |
| 02G | Food contact surface not clean | 17,308 |
| 10B | Improper utensil storage | 17,142 |
| 06C | Food not refrigerated properly | 16,733 |
| 04L | Vermin infestation | 15,200 |
| 02B | Food contaminated | 14,564 |
| 04N | Unclean surfaces | 11,317 |
| 04A | Improper hand washing | 7,746 |

---

### 🧮 Category 4: Grade Distribution  

| Grade | Count | Percentage |
|--------|--------|-------------|
| A | 92,291 | 35.13% |
| B | 17,433 | 6.64% |
| C | 11,932 | 4.54% |
| N (Not Yet Graded) | 133,677 | 50.89% |
| P (Pending) | 838 | 0.32% |
| Z (Under Review) | 6,512 | 2.48% |

Over **35% of restaurants earn an “A”**, while nearly **half remain ungraded**, often due to pending inspections or new openings.  

---

## 💡 Recommendations  

Based on the findings above, the **NYC Department of Health** should:  

1. **Target High-Risk Cuisines:** Focus on American, Chinese, and Italian restaurants with the highest violation counts.  
2. **Address Critical Violations:** Prioritize training and re-inspection around temperature control and pest management.  
3. **Seasonal Oversight:** Increase inspection frequency in warmer months to reduce pest and contamination issues.  
4. **Enhance Transparency:** Encourage timely publication of inspection results to boost public confidence.  
5. **Data Quality Improvements:** Standardize cuisine and inspection type categories for consistent analytics.  

---

### 📊 Tools & Technologies  
- **SQL (MySQL)** – Data extraction, cleaning, and aggregation  
- **Tableau / Power BI** – Visualization and dashboarding  
- **Excel & Pandas** – Exploratory analysis and data validation  

---

**Author:** Kareem Kotb  
**Project Source:** [AnalystBuilder Project – Restaurant Health Inspection Analysis NYC](https://www.analystbuilder.com/projects/restaurant-health-inspection-analysis-nyc-FhAOm)

