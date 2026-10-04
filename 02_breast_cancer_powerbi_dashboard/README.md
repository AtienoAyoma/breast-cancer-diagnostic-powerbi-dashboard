# Breast Cancer Diagnostic Feature Analysis Dashboard

## Project summary
A Power BI-ready healthcare analytics project using the UCI Breast Cancer Wisconsin (Diagnostic) dataset. The dataset contains 569 cases and 30 real-valued features derived from digitised fine-needle-aspirate images of breast masses.

## Tools
Power BI, Power Query, Excel

## Dashboard goals
- Present high-level case and diagnosis KPIs.
- Compare feature distributions between benign and malignant cases.
- Explore relationships between diagnostic features using interactive visuals.
- Demonstrate data preparation and dashboard storytelling.

## Included files
- `data/breast_cancer_wisconsin_clean.csv` — cleaned Power BI import file.
- `data/breast_cancer_dashboard_data.xlsx` — Excel workbook with clean data and summary sheets.
- `data/diagnosis_summary.csv` — grouped summary.
- `powerbi/dashboard_build_guide.md` — page layout, visual recommendations and DAX measures.
- `visualisations/` — supporting analysis visuals.

## Data source
UCI Machine Learning Repository — Breast Cancer Wisconsin (Diagnostic).
Official source: https://archive.ics.uci.edu/dataset/17/breast-cancer-wisconsin-diagnostic

## Important limitation
The dataset is historical and its features describe digitised cell-nucleus characteristics. The dashboard is for portfolio/educational analytics and must not be presented as a clinical diagnostic system.
