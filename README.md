# Customer Segmentation and Rule-Based Churn Risk Analysis

## Project overview
This project segments customers using a transparent, rule-based churn-risk score. It is designed as a beginner-friendly analytics exercise using the supplied sample customer churn dataset.

## Files
- `Task04_Customer_Segmentation.ipynb` — Python notebook for data checks, scoring, segment summaries, visualization, and validation.
- `customer_churn_sample.csv` — source dataset supplied for the task.
- `customer_segments.csv` — customer-level scores, risk bands, segments, and risk factors.
- `segment_summary.csv` — summary metrics by customer segment.
- `Task04_Recommendation_Memo.docx` — recommendations and limitations report.

## Risk-scoring rules
- Tenure of 6 months or less: +30 points.
- Tenure of 7–12 months: +20 points.
- 5 or more support tickets: +30 points.
- 3–4 support tickets: +20 points.
- Month-to-month contract: +25 points.
- Basic subscription: +10 points.
- Score is capped at 100.
- High risk: score >= 60; Medium risk: 35–59; Low risk: below 35.

## How to run
1. Open the notebook in Google Colab or Jupyter.
2. Upload `customer_churn_sample.csv` or place it in the same folder as the notebook.
3. Run the cells from top to bottom.
4. The notebook writes `customer_segments.csv` and `segment_summary.csv`.

## Important limitations
The supplied dataset contains only a small sample. The score is a transparent prioritisation heuristic, not a trained machine-learning model and not a calibrated probability of churn. Results should not be generalised without testing on a larger dataset.
