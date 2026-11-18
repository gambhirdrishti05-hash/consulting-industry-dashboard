# The Talent Crisis Behind the Consulting Boom

**Live Dashboard:** [View on Tableau Public](https://public.tableau.com/views/TheTalentCrisisBehindtheConsultingBoom/TheTalentCrisisBehindtheConsultingBoom?:language=en-US&publish=yes&:sid=&:display_count=n&:origin=viz_share_link)

## Why I built this

I spent 2 years at EY and saw the industry hire heavily and lose people quickly. I wanted to see whether public data showed a similar pattern at the market level. This dashboard looks at U.S. consulting from 2013 to 2024 and asks whether headcount growth kept pace with revenue. The data does not measure burnout, attrition or pay, so it only covers the hiring and revenue side.

## What the data shows

- The industry added about 600,000 employees in 2023, then lost about 150,000 in 2024
- Revenue per consultant fell about 23%, from $196K in 2022 to $150K in 2023, the sharpest single year drop in this dataset. It recovered to about $171K in 2024
- Deloitte's U.S. revenue grew about 40%, from roughly $23B in 2021 to roughly $33B in 2024
- The Big Four's share of the U.S. consulting market grew from 14.8% in 2013 to a peak of about 23.8% in 2023, then 22.8% in 2024

## Dashboard structure

| Chart | What it shows |
|---|---|
| U.S. Consulting Workforce 2013 to 2024 | Industry headcount over time, including the 2023 jump and the 2024 drop |
| Revenue Per Consultant 2013 to 2024 | Market revenue divided by headcount, and the 2023 drop |
| Big Four Revenue Growth 2012 to 2024 | Deloitte, PwC, EY and KPMG U.S. revenue trends |
| Big Four Share of U.S. Market 2013 to 2024 | The Big Four's share of total U.S. consulting revenue |

## Data sources

All data from Statista (2025):
- U.S. management consulting market size 2013 to 2024
- U.S. management consulting employees 2013 to 2024
- Deloitte, PwC, EY and KPMG U.S. revenue 2012 to 2024
- [Annual revenue growth of management consultancies worldwide 2015 to 2024: keep only if the dashboard uses it, otherwise delete this line]

## What I did with the data

The raw Statista files came as separate Excel exports. I merged them into one clean master file using Python, then calculated three KPIs that were not in the raw data:

- Year over year market growth %
- Revenue per employee (total market revenue divided by total industry headcount)
- Big Four market share % by year

## Tools used

- Python (pandas, openpyxl) for cleaning and merging the data
- Excel for raw data storage
- Tableau Desktop and Tableau Public for building and publishing the dashboard

## Files in this repo

| File | What it is |
|---|---|
| `consulting_kpi_master.xlsx` | The cleaned master dataset with all calculated KPIs |
| [`cleaning script name`] | [The Python script or notebook used to clean and merge the data] |
| `README.md` | This file |

## The main takeaway

In 2023, headcount rose 32% while market revenue grew about 1%, so revenue per employee fell about 23%. That is partly arithmetic: the ratio drops when headcount grows faster than revenue. Headcount then fell by about 150,000 in 2024, which is consistent with a correction, but this data cannot show why firms cut. The 2023 jump may also partly reflect how the source counts employees.

## Limits

- Industry level data only, so it says nothing about individual firms' hiring or pay
- Revenue per employee is a derived ratio (market revenue divided by headcount), not a measured productivity figure
- No attrition, burnout or pay data is included
- The 2023 headcount jump may partly reflect how the source counts employees
- [Big Four figures are U.S. revenue per firm. State here whether they cover consulting only or the whole firm, because it affects the market share figures]

## Next step

I plan to extend this analysis with U.S. Bureau of Labor Statistics hiring and separations data, joined with these tables in Snowflake using SQL.

## About me

Drishti Gambhir | MS Business Analytics, UMass Boston (2026)
[LinkedIn](https://www.linkedin.com/in/drishtigambhir) | [Tableau Public](https://public.tableau.com/views/TheTalentCrisisBehindtheConsultingBoom/TheTalentCrisisBehindtheConsultingBoom?:language=en-US&publish=yes&:sid=&:display_count=n&:origin=viz_share_link)
