# Project-1

# 🎵 Spotify Song Mood Analyzer using Mode Concept

A data science project that analyzes the mood of Spotify tracks using audio features like **valence**, **energy**, and **mode**. This project visualizes how songs differ in emotional tone and musical structure, and lets users input a track name to see its mood on a mood map.

---

## 📌 Project Highlights

✅ Categorizes songs into **Major** and **Minor** mode  
✅ Classifies song mood using **valence** (happiness) and **energy** (activeness)  
✅ Visualizes:
- Mode distribution
- Tempo distribution
- Valence vs Energy mood map
✅ Highlights a user-selected song on the mood map

---

## 📂 Dataset

- File: `spotify_data.csv`
- Required columns:  
  `track_name`, `artist`, `valence`, `energy`, `mode`, `tempo`

---

## 🛠️ Installation

```bash
pip install pandas matplotlib seaborn

```
# Project-2

# 📊 Statistical Analysis of User Behavior through A/B Testing

This project performs a statistical A/B test to analyze user conversion behavior between two groups — **Group A** and **Group B** — and determines if the difference in performance is **statistically significant** using a **Z-test for proportions**.



## 📁 Project Structure

```
├── ab_test_analysis.ipynb      # Google Colab with full code and visualizations
├── dataset.csv                 # A/B testing dataset (users, groups, conversions)
└── README.md                   # Project documentation
```
---

## 🔍 What Does `converted` Mean in A/B Testing?

| Value | Meaning                                                                 |
|--------|-------------------------------------------------------------------------|
| `1`    | ✅ **User converted** – they clicked, signed up, purchased, or performed the desired action |
| `0`    | ❌ **User did not convert** – they visited but didn't take the desired action               |

---

## 📌 Objective

- Analyze conversion rates between two different user groups (A/B).
- Use statistical testing to determine whether one group performs significantly better.
- Visualize the data through bar charts and pie charts.

---

## 🧪 Statistical Method Used

We use the **two-proportion Z-test** to evaluate:

- **Null Hypothesis (H₀)**: No difference in conversion rates between A and B.  
- **Alternative Hypothesis (H₁)**: A significant difference exists between the two groups.

---

## 📌 Explanation:
p_val < alpha: means the difference is statistically significant.

- Z-statistic tells how far apart the conversion rates are.
- P-value tells if that difference is statistically significant.
- Alpha = 0.05 means we want at least 95% confidence.

Then you check which group had the higher conversion rate:

If B > A → B is better

If A > B → A is better

## 📊 Key Steps

1. **Load and clean the dataset**
2. **Calculate total users and conversions per group**
3. **Compute conversion rates**
4. **Perform Z-test for significance**
5. **Visualize results using pie charts and bar charts**

---

## 📈 Sample Output

```
📋 === A/B Test Z-Test Summary ===
Group A Conversion Rate: 13.4%
Group B Conversion Rate: 12.2%
Z-Statistic: 0.568
P-Value: 0.5701
❌ Conclusion: No significant difference between Group A and Group B
```

---

## 📊 Visualizations

- 📎 **Pie Charts**: Show conversion vs. non-conversion distribution in each group  
- 📎 **Bar Plot**: Compare conversion rates side-by-side  
- 📎 **Z-Test Output**: Shows whether the observed difference is statistically meaningful

---

## 🧰 Technologies Used

- Python 🐍  
- Pandas 📊  
- Matplotlib & Seaborn 🎨  
- statsmodels 📐  
- Jupyter Notebook 📒  

---

## 📥 How to Run

1. Clone this repo:
```bash
git clone https://github.com/your-username/ab-testing-analysis.git
```

2. Install dependencies:
```bash
pip install pandas matplotlib seaborn statsmodels
```

3. Run the Jupyter Notebook:
```bash
Google Colab ab_test_analysis.ipynb
```

---

## 🔬 Conclusion

This project demonstrates how A/B testing and statistical inference can guide product and marketing decisions using real user data. Even small differences in conversion rates may not always be statistically significant — which is why proper testing is critical.

---

## 📄 License

MIT License © 2025 Kushvanth
