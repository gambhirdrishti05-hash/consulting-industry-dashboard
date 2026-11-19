# The Talent Crisis Behind the Consulting Boom

**Live Dashboard:** [View on Tableau Public](https://public.tableau.com/views/TheTalentCrisisBehindtheConsultingBoom/TheTalentCrisisBehindtheConsultingBoom?:language=en-US&publish=yes&:sid=&:display_count=n&:origin=viz_share_link)

## Why I built this

I spent 2 years at EY and saw the industry hire heavily and lose people quickly. I wanted to see whether public data showed a similar pattern at the market level. This dashboard looks at U.S. consulting from 2013 to 2024 and asks whether headcount growth kept pace with revenue. The data does not measure burnout, attrition or pay, so it only covers the hiring and revenue side.

## What the data shows

- U.S. consulting headcount rose by about 600,000 in 2023 (+32%), then fell by about 150,000 in 2024
- Market revenue grew less than 1% in 2023 (0.7%), so revenue per consultant fell about 23%, from $196K in 2022 to $150K in 2023. This is the sharpest single year drop in the dataset. It recovered to about $171K in 2024
- Deloitte's U.S. revenue grew about 44%, from $22.9B in 2021 to $33.1B in 2024
- Big Four U.S. revenue equaled about 14.8% of the U.S. consulting market size in 2013, peaked near 23.8% in 2023, and was 22.8% in 2024. This is a ratio of firm revenue to market size, not a true consulting market share (see Limits)

## Dashboard structure

| Chart | What it shows |
|---|---|
| U.S. Consulting Workforce 2013 to 2024 | Industry headcount over time, including the 2023 jump and the 2024 drop |
| Revenue Per Consultant 2013 to 2024 | Market size divided by headcount, and the 2023 drop |
| Big Four Revenue Growth 2012 to 2024 | Deloitte, PwC, EY and KPMG U.S. revenue trends |
| Big Four Share of U.S. Market 2013 to 2024 | Big Four U.S. revenue as a percentage of U.S. consulting market size |

## Data sources

All data from Statista (2025):
- U.S. management consulting market size and employees, 2013 to 2024 (IBISWorld)
- Deloitte, PwC, EY and KPMG U.S. revenue, 2012 to 2024

## What I did with the data

The raw Statista files came as separate Excel exports. I merged them into one master file using Python and calculated each firm's share of the Big Four total and the Big Four total revenue. Revenue per consultant (market size divided by headcount) and the Big Four to market ratio were calculated in Tableau. [Confirm this is accurate, or describe what actually happened.]

## Tools used

- Python (pandas, openpyxl) for cleaning and merging the data
- Excel for raw data storage
- Tableau Desktop and Tableau Public for building and publishing the dashboard

## Files in this repo

| File | What it is |
|---|---|
| `Consulting_KPI_Master_Dataset.xlsx` | The merged master dataset, with a data dictionary |
| [script name] | [The Python script or notebook used to merge the data] |
| `README.md` | This file |

## The main takeaway

In 2023, headcount rose 32% while market revenue grew less than 1%, so revenue per consultant fell about 23%. That is partly arithmetic: the ratio drops when headcount grows faster than revenue. Headcount then fell by about 150,000 in 2024, which is consistent with a correction, but this data cannot show why firms cut. The 2023 jump may also partly reflect how the source counts employees.

## Limits

- Industry level data only, so it says nothing about individual firms' hiring or pay
- Revenue per consultant is a derived ratio (market size divided by headcount), not a measured productivity figure
- No attrition, burnout or pay data is included
- The 2023 headcount jump may partly reflect how the source counts employees
- Firm revenues are total U.S. revenue (audit, tax, advisory and consulting), but market size covers consulting only. The Big Four ratio therefore overstates their consulting share
- PwC's 2016 revenue is missing in the source. [State how you handled it in Tableau.] The 2025 row has only Deloitte and is not used

## Next step

I plan to extend this analysis with U.S. Bureau of Labor Statistics hiring and separations data, joined with these tables in Snowflake using SQL. [Delete this section if you are not going to build it.]

## About me

Drishti Gambhir | MS Business Analytics, UMass Boston (2026)
[LinkedIn](https://www.linkedin.com/in/drishtigambhir) | [Tableau Public](https://public.tableau.com/views/TheTalentCrisisBehindtheConsultingBoom/TheTalentCrisisBehindtheConsultingBoom?:language=en-US&publish=yes&:sid=&:display_count=n&:origin=viz_share_link)
