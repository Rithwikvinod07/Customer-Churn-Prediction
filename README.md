# Customer-Churn-Prediction
This Python project creates a synthetic 20K-user dataset for streaming churn prediction, mimicking Netflix. Features: demographics, subscriptions (basic/standard/premium), usage (watch hours, inactivity), add-ons, pricing, support, lifetime value. Churn (33% rate) via probability model adjusted for engagement/inactivity/tenure.
#READ ME
Streaming Churn Prediction Project
Predict customer churn for streaming services like Netflix using a realistic synthetic dataset and comprehensive EDA.
This project generates a 20,000-user dataset (streaming_churn_20k.csv) with 21 features mimicking real streaming behavior:​

Demographics: Age (18-70), countries (US 35%, UK/IN/etc.)

Subscriptions: Tenure (1-60 months), plans (basic/standard/premium at 40/40/20%)

Usage: Watch hours (30d/7d via gamma dist.), inactivity days (0-45), genre diversity, binges

Other: Add-ons (4K/offline), pricing ($10-20), support tickets, payment failures, lifetime value​

Churn (33.4% rate) uses a smart probability model: base 15%, rising to 54% for <10 watch hours, falling for premium/long-term users.​

Key EDA Insights
Premium plans churn least (29%)

Low engagement (0-10 hrs) churns most (54%)

Top predictors: Days since last watch (corr 0.33), recent watch hours (-0.20)​

Visuals include histograms, boxplots, heatmaps via Pandas/Seaborn/Matplotlib.​

🚀 Quick Start
bash
pip install pandas numpy seaborn matplotlib
python generate_data.py  # Creates dataset
python eda_analysis.py   # Runs EDA with plots
📊 Dataset Stats
Metric	Value
Rows	20,000​
Features	21​
Churn Rate	33.37%​
Perfect for ML practice (Random Forest, XGBoost) or portfolio demos. Fork, star, and contribute!
