# OTT Subscriber Engagement & Retention Analysis

## Project Overview

This project explores subscriber viewing behaviour, content engagement, and repeat viewing using a simulated OTT dataset. The objective is to demonstrate how Python-based analytics can help investigate patterns in viewer engagement and content performance.

**Note:** The dataset is synthetic and does not represent real customer data from an OTT company.

## Business Questions

- How is early viewing engagement associated with subsequent repeat viewing?
- Which genres have higher average content-completion rates?
- How do viewing patterns vary across acquisition channels, subscription plans, and primary devices?
- What business opportunities can be investigated based on these patterns?

## Tools & Technologies

- Python
- Pandas and NumPy
- Matplotlib
- SciPy
- Kaggle Notebooks / Jupyter Notebook

## Dataset

The project uses two simulated CSV datasets:

- `subscribers.csv`: 10,000 subscriber profiles, including subscription plan, primary device, region, language, and acquisition channel.
- `viewing_sessions.csv`: 150,000 viewing-session records, including genre, content type, watch duration, completion percentage, and session date.

The data is intended for educational and portfolio use.

## Methodology

1. Data inspection and quality checks
2. Subscriber-level aggregation of viewing activity
3. Engagement segmentation by early viewing behaviour
4. Repeat-viewing analysis using the first 30 days as the engagement window and days 30–59 as the follow-up window
5. Genre, content-type, acquisition-channel, subscription-plan, and device comparisons
6. Chi-square testing and Cramér's V effect-size calculation
7. Business interpretation and recommendations

## Key Findings

### Early Engagement and Repeat Viewing

- High early-engagement subscribers had a repeat-viewing rate of **78.99%**.
- Low early-engagement subscribers had a repeat-viewing rate of **53.42%**.
- The difference was **25.57 percentage points**.
- The chi-square test returned χ² = 484.74, p < 0.001, with Cramér's V = 0.270.

These results indicate an association between early engagement and subsequent repeat viewing in the simulated data. They do not establish causality or real-world customer retention.

### Content Performance

- Thriller had the highest average completion rate at **80.01%**.
- Documentary had the lowest average completion rate at **74.44%**.
- Drama recorded the highest session volume, with **37,427 sessions**.

Completion rate and session volume measure different aspects of content performance.

### Acquisition Channels, Plans, and Devices

Differences in average viewing and repeat-viewing rates across these groups were relatively modest in the simulated dataset. Viewing behaviour alone is insufficient to determine acquisition profitability or subscription-plan performance.

## Business Recommendations

- Investigate onboarding and content-discovery experiences as potential ways to encourage repeat viewing.
- Evaluate content using multiple measures, including completion, viewing volume, repeat viewing, and cost.
- Combine acquisition costs and subscription revenue with engagement data before assessing marketing efficiency.
- Examine device-specific user experience issues without assuming that device type causes differences in repeat viewing.

## Limitations

- The data is simulated and does not represent a real OTT platform.
- Repeat viewing is not equivalent to paid-subscription retention or churn.
- The analysis is observational and cannot establish causality.
- Statistical significance in simulated data does not establish real-world business significance.

## Project Structure

```text
OTT-subscriber-engagement-retention-analysis/
├── README.md
├── OTT_Engagement_Analysis.ipynb
└── data/
    ├── subscribers.csv
    └── viewing_sessions.csv
```

## How to Run

1. Download or clone this repository.
2. Install the required Python packages: `pandas`, `numpy`, `matplotlib`, and `scipy`.
3. Open the notebook in Jupyter or upload it to Kaggle.
4. Ensure the CSV files are available at the paths used in the notebook, updating those paths if necessary.
5. Run the notebook cells in order.

## Conclusion

This project demonstrates subscriber-level aggregation, behavioural segmentation, repeat-viewing analysis, content-performance comparisons, and statistical testing. The results provide an example of an analytical workflow; validation with real subscriber and subscription-status data would be required before applying the findings to business decisions.
