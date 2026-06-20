# Aviation Workforce Analytics: Power BI Case Study

## Business Problem

A flight training academy needed to understand which factors most strongly influence trainee placement outcomes and identify opportunities to improve recruitment, training effectiveness, and airline partnerships. The goal of this analysis was to evaluate trainee performance, instructor effectiveness, and geographic recruiting trends in order to identify actionable opportunities to improve placement rates.

### Overview

**Interactive Power BI Dashboard** analyzing trainee placement outcomes for a regional aviation training academy.

## Key Findings & Insights

- **83.5% overall placement rate**. 167 of 200 trainees placed across 25 airline partners, establishing a strong performance benchmark for the academy.

- **Instructor assignment is the strongest predictor of placement success.** Charlotte Brooks and Mia Collins achieved 96.6% placement rates while Daniel Cooper achieved 67.9% — a 28.7 percentage point gap that warrants immediate attention and further investigation.

- **Training duration does not predict placement outcome.** Placed and unplaced trainees trained for nearly identical durations (18.0 vs. 18.9 months). This suggests that early intervention based on time-in-training alone would be misguided.

- **Geographic variation in placement rates is significant.** Trainees from AZ, CO, IL, LA, NY, OH, TN, VA, and WA achieved near-perfect placement rates, representing Skyborne's strongest recruitment markets. IN and MO underperform — targeted employer outreach and airline network development in these markets is recommended.

- **Balanced airline partner network.** Placements are evenly distributed across all 25 airline partners at approximately 6.7 trainees per airline, indicating no single-airline dependency risk.

- **Untapped recruitment markets identified.** Gray states on the geographic map represent regions with no current Skyborne enrollment. Expanding into these markets could diversify and grow the trainee pipeline.

## Dashboard Pages
- **Executive Overview** — High-level KPIs and placement summary
<img width="706" height="389" alt="SB" src="https://github.com/user-attachments/assets/90e1832b-80bf-41ae-a91c-9067faba90d0" />

- **Training Performance** — Duration analysis and phase breakdowns
<img width="699" height="392" alt="Screenshot 2026-06-20 144321" src="https://github.com/user-attachments/assets/669c4e87-a142-4a7e-b45d-442c4ffddb1f" />

- **Airline Placement** — Partner network and geographic distribution
<img width="701" height="394" alt="Screenshot 2026-06-20 144435" src="https://github.com/user-attachments/assets/cf4a9584-b550-4a9c-8a1f-1d7fa05c12c1" />

- **Instructor & Cohort Performance** — Instructor effectiveness analysis
<img width="701" height="394" alt="Screenshot 2026-06-20 175949" src="https://github.com/user-attachments/assets/41c2ba6b-86b5-4cc1-8c6c-d1cb468257be" />

- **Insights & Recommendations** — Key findings and strategic recommendations

## Limitations & Recommended Next Steps

| Limitation | Impact | Recommendation |
|------------|--------|----------------|
| Per-phase training duration | Only a single average phase duration per trainee was available. True phase-by-phase performance analysis was not possible. | Capture individual phase completion dates and durations in the source system. |
| Phase-level dropout analysis | Dataset records only final placement outcome with no milestone or checkpoint data. Identifying where in the pipeline trainees disengage was not possible. | Add phase completion status fields to track dropout points in real time. |
| Time to placement after graduation | No graduation date or hire date fields exist. Average time between program completion and airline placement could not be calculated. | Add graduation date and first day of employment fields to enable this metric in a future iteration. |
| Demographic analysis | No demographic fields such as age, educational background, or prior aviation experience exist. Cohort analysis was limited to geography, training duration, and instructor assignment. | Consider collecting relevant background data at enrollment to enable richer cohort segmentation. |



## Technical Details
- Built in **Microsoft Power BI Desktop**
- 16 custom DAX measures in a dedicated measures table
- Semantic data model with star schema architecture
- Synthetic dataset of 200 trainees
- Data cleaning performed in Power Query
- Calculated placement-rate measures
- Built geographic mapping visuals
- Created instructor-performance comparisons
- Designed interactive filtering across pages

## Tools Used
- Power BI Desktop
- DAX
- Power Query
- SQL (data preparation)

## Repository Contents
- `Skyborne_Case_Study.pbix` — Main Power BI file
- `Documentation/` — Methodology and full insights PDF
