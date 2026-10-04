# Power BI Dashboard Build Guide

## Page 1 — Executive Overview
**KPI cards**
- Total Cases
- Benign Cases
- Malignant Cases
- Malignant %

**Charts**
1. Clustered column: Cases by Diagnosis
2. Donut: Diagnosis share
3. Scatter: Mean Radius vs Mean Texture, legend = Diagnosis
4. Column chart: Average Mean Radius by Diagnosis

**Slicers**
- Diagnosis

## Page 2 — Feature Analysis
Use a matrix/table for selected feature averages and scatter plots for relationships such as:
- Mean Radius vs Mean Perimeter
- Mean Radius vs Mean Area
- Worst Radius vs Worst Texture

## DAX measures
```DAX
Total Cases = COUNTROWS(Clean_Data)

Benign Cases = CALCULATE([Total Cases], Clean_Data[Diagnosis] = "Benign")

Malignant Cases = CALCULATE([Total Cases], Clean_Data[Diagnosis] = "Malignant")

Malignant % = DIVIDE([Malignant Cases], [Total Cases])

Average Mean Radius = AVERAGE(Clean_Data[Mean Radius])

Average Mean Texture = AVERAGE(Clean_Data[Mean Texture])

Average Mean Area = AVERAGE(Clean_Data[Mean Area])
```

## Suggested dashboard title
**Breast Cancer Diagnostic Feature Analysis**

## Interpretation note
This is an educational analytics project using a historical public dataset. It demonstrates data preparation and visual analysis; it is not a clinical diagnostic tool and should not be presented as one.
