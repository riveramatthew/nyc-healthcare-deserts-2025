# Where You Live Determines If You Get Care  
## Mapping Healthcare Deserts in New York City (STA 9750 – Fall 2025)

![Healthcare Access Score Map](images/figure4-access-score-map.png)

**One in six New Yorkers lives in a healthcare desert.**  
This repository contains the complete, reproducible analysis showing that geographic access to hospitals, clinics, and urgent care in NYC is deeply unequal — and overwhelmingly concentrated in low-income, majority-minority, and immigrant neighborhoods.

### Overarching Question
**How does geographic access to healthcare facilities vary across NYC at the census-tract level, and what socioeconomic disparities exist in healthcare access?**

### Team
- Matthew – Geographic Distribution & Walking Distance Modeling  
- Imani – Borough/ZIP-Level Supply Analysis  
- Jason – Income, Cost Barriers & Delayed Care  
- Zhuohan – Race, Poverty & Multivariate Correlations  
- Saoni – Immigration Status, Language, and Insurance Gaps  

### Final Deliverables
- [Group Summary Report (non-technical)](docs/summary-report.html) – 2,013 words  
- Individual Technical Reports (reproducible Quarto) – see `/reports/`  
- [Interactive Dashboard (live maps)](https://nyc-healthcare-deserts-2025.netlify.app)  
- All presentations (proposal → mid-semester → final)

### Quick Start (Reproduce Everything)
```r
# 1. Clone repo
git clone https://github.com/yourusername/nyc-healthcare-deserts-2025.git
cd nyc-healthcare-deserts-2025

# 2. Open in RStudio → opens .Rproj automatically
# 3. Run the pipeline
source("src/01-download-data.R")
source("src/02-clean-facilities.R")
# ... continue through 05-analysis-*.R

# 4. Render reports
quarto render reports/group-summary.qmd
quarto render reports/individual-*.qmd
