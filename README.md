# YouTube Views Prediction 🎥📊

This project explores whether we can **predict the number of views a YouTube video will get** using only metadata available at upload time (title, description, tags, publish time, channel stats, etc.).  
Spoiler: predicting virality is hard with so many different factors that come in to play

---

## 🚀 Project Overview
- Dataset: [YouTube Trending Video Dataset (US)](https://www.kaggle.com/datasets/datasnaek/youtube-new)
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

➡️ **Interpretation**: YouTube virality is influenced by factors such as thumbnail, and actual video content that are not captured in metadata. This makes getting an accurate prediction from meta-data often impossible.  

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
- Real-world data is messy and will often not end up how we want it to.  
- Some prediction tasks may simply not be possible with the data that is provided.  
- Even "low-performing" models reveal insights about data limitations.  
