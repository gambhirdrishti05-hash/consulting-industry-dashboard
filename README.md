# The Talent Crisis Behind the Consulting Boom

**Live Dashboard:** [View on Tableau Public](https://public.tableau.com/views/TheTalentCrisisBehindtheConsultingBoom/TheTalentCrisisBehindtheConsultingBoom?:language=en-US&publish=yes&:sid=&:display_count=n&:origin=viz_share_link)

## Why I built this

I spent 2 years at EY and watched the industry hire in mass and burn people out. People were leaving as fast as they were being brought in. The pay wasn't matching the pressure. I wanted to see if the numbers backed what I experienced firsthand. They did.

This dashboard looks at the U.S. consulting industry between 2013 and 2024 and asks one question: is the way these firms grow actually sustainable?

## What the data shows

- The industry added 600,000 employees in 2023, then lost 150,000 the very next year
- Revenue per consultant dropped from $197K in 2022 to $150K in 2023 — the sharpest single-year fall in the decade
- Deloitte's U.S. revenue nearly doubled from $23B to $33B between 2021 and 2024
- The Big Four's share of the total U.S. consulting market grew from 14.8% in 2013 to 23.8% in 2023

## Dashboard structure

| Chart | What it shows |
|---|---|
| U.S. Consulting Workforce 2013–2024 | Industry headcount over time, highlighting the 2023 surge and 2024 drop |
| Revenue Per Consultant 2013–2024 | How much revenue each consultant generated — and when it collapsed |
| Big Four Revenue Growth 2012–2024 | Deloitte, PwC, EY, KPMG revenue trends and how far Deloitte pulled ahead |
| Big Four Share of U.S. Market 2013–2024 | How much of the total market the Big Four control, and how fast that's growing |

## Data sources

All data from Statista (2025):
- U.S. management consulting market size 2013–2024
- U.S. management consulting employees 2013–2024
- Annual revenue growth of management consultancies worldwide 2015–2024
- Deloitte, PwC, EY, KPMG U.S. revenue 2012–2024

## What I did with the data

The raw Statista files came as separate Excel exports. I pulled them together into one clean master file using Python. Along the way I calculated a few KPIs that weren't in the raw data:

- Year-over-year market growth %
- Revenue per employee (total market revenue divided by total industry headcount)
- Big Four market share % by year

## Tools used

- Python (pandas, openpyxl) — cleaning and merging the data
- Excel — raw data storage
- Tableau Desktop and Tableau Public — building and publishing the dashboard

## Files in this repo

| File | What it is |
|---|---|
| `consulting_kpi_master.xlsx` | The cleaned master dataset with all calculated KPIs |
| `README.md` | This file |

## The main takeaway

The 2023 hiring surge wasn't backed by revenue growth. The market grew less than 1% that year but headcount jumped 32%. Revenue per consultant collapsed as a direct result. The 150K headcount reduction in 2024 was the inevitable correction. The firms that came out ahead were the ones — mainly Deloitte — that had already built enough scale to absorb the volatility. For everyone else, it exposed how thin the margins on talent really are.

## About me

Drishti Gambhir | MS Business Analytics, UMass Boston (2026)  
[LinkedIn](https://www.linkedin.com/in/drishtigambhir) | [Tableau Public](https://public.tableau.com/views/TheTalentCrisisBehindtheConsultingBoom/TheTalentCrisisBehindtheConsultingBoom?:language=en-US&publish=yes&:sid=&:display_count=n&:origin=viz_share_link)
