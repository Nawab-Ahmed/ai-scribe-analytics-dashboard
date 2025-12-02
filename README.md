# AI Scribe Analytics Dashboard (Healthcare Productivity Insights)

This project analyzes AI documentation usage across healthcare providers and specialties. It measures AI adoption, documentation time saved, provider performance, and session activity, and presents results through a 3-page Power BI dashboard following real industry practices.

## Business Problem

"How much documentation time do healthcare providers save using AI? Which provider groups benefit most, and how can leadership improve adoption?"

Healthcare systems want objective analytics to evaluate:

- AI usage frequency
- Time saved using AI Scribe
- Provider productivity
- Specialty-level performance
- High and low adoption patterns
- AI event usage (summary, transcription, rewrite, etc.)

This project solves these questions end-to-end.

## Dashboard Overview

## Page 1: Executive Summary
- Overall AI adoption
- Time saved per visit
- Total documentation hours saved
- Most used AI events
- Trend of sessions over time

## Page 2: Specialty-Level Insights
- Session distribution by specialty
- AI adoption comparison
- Average time saved per provider
- Scatter analysis for productivity

## Page 3: Provider-Level Performance
- Per-provider documentation time
- High vs low adopters
- Benchmark lines (average 50–54 seconds)
- Performance quadrants
- Provider outlier analysis

Screenshots are included in /docs/screenshots/.

## Dataset Overview

| Column | Description |
|--------|-------------|
| session_id | Unique session identifier |
| provider_id | Physician / clinician ID |
| specialty | Medical specialty |
| ai_event_type | AI Summary / Rewrite / Transcript / etc |
| ai_doc_time_per_visit | AI documentation time |
| manual_doc_time_per_visit | Manual documentation time |
| time_saved_per_visit | Derived metric |
| session_datetime | Day and time of session |

A sample dataset is included (dummy only; real data confidential).

## Methods Used

- Data cleaning (Pandas)
- Exploratory data analysis (Python)
- Time savings calculation
- AI event usage frequency analysis
- Provider and specialty benchmarking
- Power BI visual storytelling
- KPI design
- User-centric dashboard layout

## Tech Stack

- Python (Pandas, NumPy, Matplotlib)
- Power BI (DAX, model design, KPI development)
- Git and GitHub
- Excel
- Jupyter Notebooks

## Key Insights

- Average time saved per visit: 50–54 seconds
- Certain specialties show much higher AI adoption than others
- Top-performing providers complete documentation 30–40% faster
- AI Summary is the most frequently used event type
- Large variance in provider efficiency highlights training opportunities
