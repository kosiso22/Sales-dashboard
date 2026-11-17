# Sales & Client Sentiment Review — Power BI Dashboard

A two-page Power BI dashboard built on a fictional retail dataset,
pulling together sales performance and client sentiment (social media
engagement) into one view.

## What it shows

**Page 1 — Sales Performance Review**
Total revenue, average sale, total quantity sold, total cost, gross
margin %, and year-on-year revenue growth, with a breakdown of revenue
by branch.

**Page 2 — Client Engagement Review**
Total engagements, overall sentiment score and average sentiment score,
with engagement volume broken down by branch, plus filters by topic and
channel (e.g. Twitter, Facebook, Instagram, TikTok, web reviews).

A preview of both pages (as a PDF export) is included in this repo in
case you don't have Power BI Desktop installed — see `dashboard_preview.pdf`.

## Data

`sales_data.xlsx` is the dataset behind the dashboard. It's fully
fictional, built as part of a school(university) assignment, and contains five sheets:

| Sheet | Contents |
|---|---|
| `Branches` | Branch code, city, province, floor space, staff count |
| `Inventory` | Products, categories, cost price, selling price |
| `Customers` | Anonymised customer IDs (no real names), type, province |
| `Sales` | Transaction-level sales records linking branches, products and customers |
| `Social media` | Posts, channel, sentiment score, topic and engagement count by branch |



## Files

```
sales_client_sentiment_dashboard.pbix    the Power BI file (open in Power BI Desktop)
sales_data.xlsx                          the underlying dataset
dashboard_preview.pdf                    a static export of both pages
```

## Opening it

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (Windows only).
2. Open `sales_client_sentiment_dashboard.pbix`.
3. If Power BI asks you to point it at the data source, redirect it to
   your local copy of `sales_data.xlsx` (**Home → Transform data → Data
   source settings → Change Source**) — the original file path baked
   into the report belonged to the machine it was built on, so Power BI
   won't find it automatically on a different computer.

If you just want to see what it looks like without installing anything,
open `dashboard_preview.pdf`.

## Tools used

Power BI Desktop, Excel.

## Why this exists

Built as a mini project to practice turning a messy, multi-sheet
dataset into a dashboard that tells a story on two fronts. How the
business is performing, and how customers feel about it, rather than
just reporting numbers in isolation.
