# AI Analytics Copilot

## Project Overview

Built a token-efficient AI-powered analytics copilot using Python, Pandas, and the OpenAI API to analyze business datasets and generate executive-ready insights.

The system automatically detects dataset structure, identifies meaningful business metrics, performs anomaly detection, concentration analysis, correlation analysis, and segment analysis, then uses OpenAI to generate leadership-friendly summaries and recommended business actions.

Instead of sending full datasets to the LLM, the project uses a token-efficient architecture by sending only aggregated summaries, improving speed, reducing cost, and minimizing hallucination risk.

---

## Business Problem

Traditional dashboards show what happened, but leadership often needs help understanding:

- What should we investigate first?
- Where are the hidden risks?
- Are we overly dependent on one segment?
- Which anomalies deserve immediate attention?

This project acts as an AI decision-support copilot by helping analysts move from descriptive analytics to diagnostic insights.

---

## Key Features

- Automatic dataset type detection
- Smart exclusion of ID-like fields (order_id, customer_id, etc.)
- Primary business metric selection
- Numeric and categorical summaries
- Missing value detection
- High/low anomaly detection
- Concentration risk analysis
- Correlation analysis
- Segment-level performance analysis
- Token-efficient OpenAI prompt design
- Executive summary generation
- Interactive business Q&A using summarized data only

---

## Tech Stack

- Python
- Pandas
- Matplotlib
- Google Colab
- OpenAI API (gpt-4.1-mini)
- GitHub

---

## Example Business Questions

- What are the biggest operational risks in this dataset?
- Is the business overly dependent on one segment?
- Which anomalies require immediate investigation?
- What should leadership investigate next?
- Are there any data quality concerns affecting decision-making?

---

## Example Insight Generated

The West region contributes 42% of total revenue, creating concentration risk if performance declines. Discount-heavy transactions show weaker average order value, suggesting pricing inefficiency. Inventory anomalies in two stores indicate potential stockout risk and require immediate review.

---

## Why This Project Is Different

Most AI analytics projects send full datasets to an LLM and ask for generic summaries.

This project separates responsibilities:

### Python handles

- computation
- aggregation
- anomaly detection
- analysis logic

### OpenAI handles

- interpretation
- executive storytelling
- follow-up recommendations

This creates a more scalable, cost-efficient, and reliable analytics workflow.

---

## How to Run

### Step 1

Open the notebook in Google Colab

### Step 2

Create a Colab Secret named:

OPENAI_API_KEY

and add your OpenAI API key

### Step 3

Upload the provided sample CSV dataset:

retail_ai_project_dataset.csv

### Step 4

Run all cells

### Step 5

Ask business questions and review AI-generated executive insights

---
