# ⚽ Premier League Match Outcome Prediction

Machine learning project to predict outcomes of English Premier League matches.  
- **Training:** Seasons 2020–2021  
- **Testing:** Season 2022  

---

## 📊 Dataset
- **Size:** 1,389 matches × 28 columns  
- **Features:** match info (date, venue, round), teams, results, goals, xG stats, shots, possession, etc.  
- **Target:** `result` → Win (1) vs. Not-Win (0)  

---

## ⚙️ Method
- **Preprocessing:** encoded categorical features, created binary target  
- **Baseline Model:** Random Forest with predictors → venue, opponent, time, weekday  
- **Improved Model:** added rolling averages of last 3 matches (goals, shots, xG, etc.)  

---

## 📈 Results
- **Baseline Accuracy:** ~65%  
- **With Rolling Averages:** small accuracy gain, improved precision  

---

## 🚀 How to Run
```bash
pip install -r requirements.txt
jupyter notebook football_prediction.ipynb
