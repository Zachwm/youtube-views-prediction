# YouTube Views Prediction 🎥📊

This project explores whether we can **predict the number of views a YouTube video will get** using only metadata available at upload time (title, description, tags, publish time, channel stats, etc.).  
Spoiler: predicting virality is hard but the project demonstrates **end-to-end data science skills**: cleaning, feature engineering, model building, and evaluation.

---

## 🚀 Project Overview
- Dataset: [YouTube Trending Video Dataset (US)](https://www.kaggle.com/datasets/rsrishav/youtube-trending-video-dataset)
- Goal: Predict video view counts from metadata.
- Models: Random Forest (initial), [CatBoost Regressor](https://catboost.ai) (final).
- Metrics: MSE, MAE, R².

---

## 🔨 Features Engineered
- **Title & description**
  - Length, word count, sentiment (TextBlob)
- **Tags**
  - Number of tags
- **Publish time**
  - Hour of day
- **Trending timeline**
  - Day of week, month, year
- **Channel**
  - Number of videos by channel in dataset

---

## 📊 Results
| Metric | Score |
|--------|-------|
| Mean Squared Error | 3.29e13 |
| Mean Absolute Error | 1.35e6 |
| R² Score | 0.06 |

➡️ **Interpretation**: YouTube virality is influenced by external factors (promotion, algorithm, trends) that are not captured in metadata. This makes accurate prediction extremely challenging.  

---

## 🧰 Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- CatBoost
- TextBlob (NLP)
- Matplotlib

---

## 📈 Lessons Learned
- Real-world data is messy — preprocessing and feature engineering are crucial.  
- Some prediction tasks (like video virality) may be **inherently noisy**.  
- Even "low-performing" models reveal insights about data limitations.  

---

## 📂 Repository Structure
