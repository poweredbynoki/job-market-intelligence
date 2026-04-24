# Job Market Intelligence

Analyzing real SF data analyst job postings using the Adzuna API. Built this to answer a simple question: what skills do companies actually require, and is AI showing up yet?

## What this is

I pulled 246 live job postings for data analyst roles in San Francisco using Python and a free API. The goal was to stop guessing which skills to prioritize and just look at the data.

## What I found

- 244 out of 246 postings had salary data listed
- Median salary midpoint: $144,500
- AI terms like LLM, generative AI, and ChatGPT appeared in the first 500 characters of job descriptions, meaning companies are leading with AI requirements, not burying them

## A note on the skill percentages

The Adzuna free tier caps job descriptions at 500 characters. That truncation cuts off most postings before they get to the requirements section, so skill match percentages look artificially low. SQL is definitely in more than 2% of data analyst jobs. The salary data came through clean though, and the AI term findings are valid since those showed up early in descriptions.

## Stack

- Python
- Pandas
- Plotly
- Adzuna Jobs API (free tier)
- Google Colab

## Files

| File | What it is |
|------|------------|
| `job_market_intelligence.ipynb` | Full analysis notebook |
| `skills_chart.html` | Interactive skill frequency chart |
| `jobs_raw.csv` | Raw data pulled from API |
| `newplot.png` | Snapshot of skills chart |
[View live chart](https://poweredbynoki.github.io/-job-market-intelligence/skills_chart.html)

## How to run it

1. Get a free API key at [developer.adzuna.com](https://developer.adzuna.com)
2. Open the notebook in Google Colab
3. Add your `ADZUNA_APP_ID` and `ADZUNA_APP_KEY` to Colab Secrets (key icon in sidebar)
4. Run all cells top to bottom

## Why I built this

I was job searching and didn't want to rely on boot camp skill lists or blog posts. Treated my own job search as a research question, pulled real data, and made decisions based on what I found. The AI findings specifically changed how I'm positioning myself.
