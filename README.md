# Austin Crime Clearance Analysis

This project answers two questions about crimes the Austin Police Department (APD) solves:

1. How do the clearance rate and the time to clearance differ across crime categories and council districts?
2. Are incidents that are reported later less likely to be cleared?

| Finding | Result |
|---|---|
| Overall clearance rate | 13.3% of incidents with a known status (4,336 of 32,718) |
| By crime category | 94.7% for murder, 62.7% for robbery, 7.3% for theft (65% of all incidents) |
| By council district | 17.2% in District 4 down to 6.7% in District 10; low-rate districts have more thefts |
| Time to clearance | Median 1 day overall, but 81.5 days for rape |
| By reporting delay | 33.3% when reported within 1 hour, 3.2% when reported 1 to 7 days later |

## Topics Covered

- Filtering a 2.7-million-row public dataset down to one year
- Data wrangling: selecting, renaming, recoding and creating variables
- Parsing dates and date-times, and computing time differences
- Handling missing and impossible values
- Grouped summaries and reshaping tables
- Exploratory data analysis: bar plots, histograms, boxplots and small multiples on log scales

## R Packages Used

- `tidyverse`, mainly:
  - `readr`: loading the CSV
  - `dplyr`: filtering, grouping and summarizing
  - `tidyr`: reshaping tables
  - `lubridate`: dates and times
  - `forcats`: ordering categories in charts
  - `ggplot2`: charts
- `rmarkdown` and `knitr`: building the PDF report

Files:
- `Austin Crime Clearance Analysis.Rmd`: Code and text
- `Crime_Reports_2025.csv`: The 2025 incidents, exported from the portal on October 9, 2026