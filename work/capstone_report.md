# Capstone Report — Ranking Signal Analysis

- **Author:** <Your Name>
- **Lane:** Ranking Signal Analysis
- **Repo:** https://github.com/<your-username>/<repo-name>
- **Date:** July 2026

---

# 0. Abstract

This project studies which search performance signals are associated with higher visibility and engagement. The analysis uses the FlyRank Internship Warehouse dataset and focuses on March 2026. A simple descriptive analysis was performed using Google Search Console and GA4 metrics. The results identify content with high impressions, clicks and engagement. The goal is to provide simple recommendations for content optimization.

---

# 1. Problem framing

The goal of this project is to support content optimization decisions.

The unit of analysis is one content item for one client on one day.

The output is a ranking signal analysis.

The analysis helps identify pages that perform well and pages that may require improvement.

A wrong decision may lead to spending time improving pages that are already performing well while ignoring pages with better opportunities.

---

# 2. Data safety

Dataset:

- FlyRank Internship Warehouse

Main table:

- fact_content_daily_performance

Time window:

- March 2026

Features used:

- gsc_impressions
- gsc_clicks
- gsc_avg_position
- ga4_sessions
- ga4_engaged_sessions

Excluded:

- Client identifiers as predictive features.
- Future information.
- Any client-identifying information.

No client names or private information are included in this project.

---

# 3. Baseline

The baseline ranks content by Google Search impressions.

Pages with higher impressions are assumed to have greater search visibility.

This simple baseline provides a reference for later improvements.

---

# 4. Model / analysis

This project uses exploratory data analysis instead of a machine learning model.

The analysis focuses on:

- impressions
- clicks
- average position
- sessions
- engaged sessions

Simple SQL queries and summary statistics are used to study search performance.

---

# 5. Evaluation

The analysis uses March 2026 data.

Average metrics and summary statistics are reported.

Top-performing pages are identified using impressions and clicks.

Results are descriptive and intended for decision support.

---

# 6. Interpretation

Pages with higher impressions generally receive more clicks.

Pages with low clicks despite high impressions may represent optimization opportunities.

Average search position is useful for identifying pages with weaker visibility.

The analysis provides directional insights rather than causal conclusions.

---

# 7. Recommendation

Based on this analysis:

1. Monitor pages with high impressions but low clicks.
2. Improve pages with poor average position.
3. Continue monitoring high-performing pages.
4. Review engagement metrics for important pages.

These recommendations should support editorial decisions rather than replace human judgment.

---

# 8. Reproducibility

Environment:

- Python
- DuckDB
- Hugging Face Hub
- Google Colab

The notebook can be executed from top to bottom using Runtime → Run all.

Random seeds are not required because no machine learning model is trained.

---

# 9. Acknowledgments & data credit

Built on the FlyRank ML Internship dataset.

https://flyrank.ai
