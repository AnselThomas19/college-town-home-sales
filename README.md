# College-Town Home Sales Dashboard

## What this site is for

A one-page dashboard that compares home sales across the 18 cities and 11 campus areas in the College-town home sales dataset. It shows the median sale price, median price per square foot and median days on market for each city, with a filter by campus area. It is meant for anyone curious how housing near Illinois compares with other college towns, and it sets up the data for the final project.

## Live site

https://anselthomas19.github.io/college-town-home-sales/

## Data notes

- The page reads `data/college_town_home_sales.csv` in the browser and computes every number from it. Nothing is typed in by hand.
- Sales under $10,000 are left out of every figure (40 of 35,442 rows). All other prices are kept, and the page reports medians, which very high prices barely move.
- Price per square foot uses only sales with a living area above 0 sq ft (127 rows have 0).
- Days on market is `contract_date` minus `list_date`, only for sales with both dates. Blanks are not treated as zero. The table shows each city's share of sales with a list date, since homes sold without a listing are left out of this figure.
- Rows are keyed by `listing_id` and never deduplicated by address.
- `home_type` is not used because it is unreliable.
- Campus area comes from the `university` column (nearest campus by coordinates).

## Tools we used

- Claude (Anthropic) as the coding agent
- Plain HTML, CSS and JavaScript
- PapaParse 5.4.1 (loaded from jsDelivr) to read the CSV
- GitHub Pages, published by the template's workflow

## Citation

College-town home sales dataset, version 1.0 (2026). University of Illinois-Deloitte Foundation Center for Business Emerging Technologies. Data collected March 2026.
