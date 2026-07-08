# Assessing the Impact of Mental Health Influencers in Saudi Arabia

A data science project analyzing YouTube & TikTok content to understand how mental health influencers in Saudi Arabia drive audience engagement.

## 📌 Overview

Social media platforms have become powerful spaces for discussing mental health in Saudi Arabia. This project collects, cleans, and analyzes content from mental health influencers to uncover engagement patterns and build predictive models.

## 🎯 Objectives

- How does engagement differ between YouTube and TikTok for mental health content?
- Which content features (views, likes, comments, video length) most influence engagement?
- How do influencer tiers (Nano, Micro, Macro) impact audience interaction?
- What mental health topics generate the highest engagement?
- Can machine learning models accurately predict engagement performance?

## 📊 Dataset

- **Total videos:** 3,713
- **YouTube:** 3,336 videos
- **TikTok:** 377 videos
- **Time span:** 2019 – 2025
- **Language:** Arabic
- **Features:** Views, Likes, Comments, Shares, Duration, Influencer Tier, Content Type

Data was collected via the YouTube Data API and TikTok scraping (RapidAPI).

## 🗂️ Project Structure

```
├── DataCollection.ipynb          # Collecting data from YouTube & TikTok APIs
├── Cleaning_Preprocessing.ipynb  # Data cleaning, feature engineering, merging datasets
├── Poster.pdf                    # Project summary poster
└── README.md
```

## 🔍 Key Findings

- TikTok shows higher engagement efficiency despite lower content volume
- YouTube contains a larger volume of content overall
- Engagement distribution is highly skewed (a few viral videos dominate)
- Strong correlation between views and likes
- Top content topics: General Awareness, Self-development, Anxiety & Stress

## 🤖 Modeling

Multiple ML models were tested to predict engagement, including Linear Regression and Random Forest.

- **Best model:** Random Forest (R² = 0.68)
- Platform type, content format, and video length were the strongest predictors
- Short-form TikTok content showed higher engagement efficiency than longer YouTube content

## ✅ Conclusion

- Social media plays a major role in increasing mental health awareness in Saudi Arabia
- TikTok is more effective for engagement, especially for short videos
- Micro and Macro influencers have the strongest impact
- Data-driven insights can help organizations and creators design more effective mental health content

## 🛠️ Tech Stack

- Python (pandas, numpy, scikit-learn)
- YouTube Data API v3
- TikTok API (RapidAPI)
- Google Colab

## ⚙️ Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/<username>/<repo-name>.git
   ```
2. Install dependencies:
   ```bash
   pip install google-api-python-client pandas openpyxl deep-translator requests scikit-learn
   ```
3. Add your API keys as environment variables (never hardcode them):
   ```bash
   export YOUTUBE_API_KEY="your_key_here"
   export RAPIDAPI_KEY="your_key_here"
   ```
4. Run the notebooks in order: `DataCollection.ipynb` → `Cleaning_Preprocessing.ipynb`

## 👥 Team

**Prepared by:** Maryam Almazyad, Leen Almoqhim, Adhwaa Alhuzzani, Shatha Marzuq
**Supervised by:** Mashael Aldayel

---
*Towards a healthy, aware, and thriving society* 🌱
