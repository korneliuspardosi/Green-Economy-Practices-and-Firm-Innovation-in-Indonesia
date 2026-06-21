# Green Economy Practices and Firm Innovation in Indonesia
Econometric analysis of the impact of Green Economy Practice (GEP) adoption on firm-level innovation among Indonesian manufacturing and service firms using the WBES 2023 dataset and Binary Logistic Regression.

# The Impact of Green Economy Practices on Firm Innovation: Evidence from Indonesian Manufacturing and Service Sectors (2023)

## Project Overview

This repository contains the code, derived data, and econometric analysis manuscript investigating whether the adoption of Green Economy Practices (GEP) increases the likelihood of product and process innovation among Indonesian firms.

Utilizing the **2023 World Bank Enterprise Survey (WBES)** dataset for Indonesia, this study focuses on firms in the manufacturing, retail, and other services sectors that completed the Green Economy Transition (GET) module. GEP adoption is measured as an unweighted composite index across 10 specific environmental practices, including:

1. **Machinery upgrades** and **waste minimization** (most widely adopted)
2. **Lighting improvements** and **vehicle fleet upgrades**
3. **On-site green energy generation**, **heating & cooling improvements**, and **pollution control** (least adopted)

**Key Findings:** GEP adoption has no statistically significant effect on product innovation, suggesting that translating green capabilities into new commercial offerings requires broader enabling conditions — including R&D infrastructure and university-industry linkages — largely absent in Indonesia's current industrial ecosystem. In contrast, each additional green practice adopted raises the probability of process innovation by approximately **7.46 percentage points** against a baseline mean of just 2.14%, an effect concentrated among smaller and older firms. With the average Indonesian firm having adopted only roughly two of ten possible green practices and a majority adopting none, Indonesia's green innovation transition remains deeply nascent.

## Methodology

This project employs a binary discrete choice econometric approach:

- **Primary Model:** Binary Logistic Regression (Logit)
- **Robustness Check:** Probit estimation to verify distributional assumption independence
- **Interpretation:** Average Marginal Effects (AME) to quantify absolute probability changes
- **Weights:** Survey sampling weights (*wmedian_BR*) to ensure population-representative estimates
- **Standard Errors:** Heteroskedasticity-consistent (HC1) throughout
- **Controls:** Firm size (ln), firm age (ln), financial access (CFL), foreign ownership (FO), and Sector Fixed Effects (manufacturing as reference category)

## Repository Structure

```
├── notebooks/        # R scripts for data cleaning, EDA, and regression modeling
├── paper/            # Final manuscript (LaTeX source and PDF)
└── data/             # WBES Indonesia 2023 Version B dataset (.dta)
```

## Main References

- Phan, Q. (2026). The impact of green economy practices on firm innovation using data from the World Bank Enterprise Surveys. *Discover Sustainability*. https://doi.org/10.1007/s43621-026-03226-5
- Porter, M. E., & van der Linde, C. (1995). Toward a new conception of the environment-competitiveness relationship. *Journal of Economic Perspectives*, 9(4), 97–118.
- Barney, J. (1991). Firm resources and sustained competitive advantage. *Journal of Management*, 17(1), 99–120.
- Horbach, J. (2008). Determinants of environmental innovation: New evidence from German panel data sources. *Research Policy*, 37(1), 163–173.
- Ambec, S., & Lanoie, P. (2008). Does it pay to be green? A systematic overview. *Academy of Management Perspectives*, 22(4), 45–62.

## Authors

Kornelius Hasiholan Pardosi, Nathaniel Toga Siringo Ringo, William Philip Karnadi

*Faculty of Economics and Business, University of Indonesia*
