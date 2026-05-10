# ⚽ World Cup 2018 — Team Analysis using FIFA 18 Data

An in-depth analysis of the top national teams competing in the **2018 FIFA World Cup**, using the **FIFA 18 player dataset**. The project explores player ratings, market values, wages, and optimal squad formations for 10 major contenders.

---

## 📌 Project Overview

This project uses FIFA 18 player statistics to analyze and compare World Cup 2018 contenders. It identifies each team's best possible lineup across multiple formations — both based on **current overall rating** and **future potential** — and concludes with a head-to-head comparison of all 10 nations.

---

## 📂 Dataset

- **Source:** [Kaggle — FIFA 18 Complete Player Dataset](https://www.kaggle.com/datasets/thec03u5/fifa-18-demo-player-dataset)
- **File used:** `CompleteDataset.csv`
- **Key columns used:** `Name`, `Age`, `Nationality`, `Overall`, `Potential`, `Club`, `Value`, `Wage`, `Preferred Positions`

---

## 🔍 Analysis Breakdown

### 1️⃣ Data Preparation
- Loaded and filtered relevant columns from the FIFA 18 dataset
- Converted `Value` and `Wage` from string format (e.g., `€105M`, `€565K`) to numeric values
- Extracted primary preferred position for each player

### 2️⃣ Data Visualization
- **Age distribution** — histogram of player age groups
- **Overall rating distribution** — count of players by rating
- **Position distribution** — breakdown of players by field position
- **Nationality map** — interactive choropleth map showing player counts by country
- **Top 20 by Value** — HTML table of highest-valued players
- **Top 20 by Wage** — HTML table of highest-earning players
- **Scatter plots** — player value and wage vs. age and overall rating

### 3️⃣ Best Squad Analysis

Built a custom algorithm to generate the **best possible 11-player lineup** for any formation and nationality, optimizing for either **Overall** or **Potential** rating.

#### Formations analyzed:
| Formation | Description |
|---|---|
| 4-3-3 | Attacking wide play |
| 4-4-2 | Classic balanced |
| 4-2-3-1 | Deep midfield control |
| 4-3-1-2 | Twin strikers |
| 3-4-3 | Wing-heavy attack |

#### Teams analyzed:
🇫🇷 France · 🇩🇪 Germany · 🇪🇸 Spain · 🏴󠁧󠁢󠁥󠁮󠁧󠁿 England · 🇧🇷 Brazil · 🇦🇷 Argentina · 🇧🇪 Belgium · 🇵🇹 Portugal · 🇺🇾 Uruguay · 🇭🇷 Croatia

### 4️⃣ Final Comparison
Compared all 10 teams across three metrics:
- **Average Overall Rating**
- **Total Squad Market Value (€M)**
- **Average Player Wage (€K/week)**

---

## 🏆 Key Conclusions

- 🥇 **Spain** has the highest average overall rating and highest average wages
- 💰 **Germany** has the highest total squad market value (€502M)
- 🌟 **Brazil** and **Germany** follow Spain closely in overall ratings
- 🇺🇾 **Uruguay** and 🇭🇷 **Croatia** punch above their weight despite lower squad values

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3 | Core language |
| Pandas | Data manipulation |
| NumPy | Numerical operations |
| Matplotlib | Bar/scatter plots |
| Seaborn | Count plots |
| Plotly | Interactive choropleth map |
| Geopy | Geocoding support |
| Google Colab | Development environment |

---

## 🚀 How to Run

### Option 1 — Open in Google Colab
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

*(Replace with your actual Colab notebook link)*

### Option 2 — Run Locally
```bash
git clone https://github.com/anshu1516/Data-Analysis-using-Python.git
cd Data-Analysis-using-Python

pip install pandas numpy matplotlib seaborn plotly geopy

jupyter notebook World_Cup_2018_Team_Analysis.ipynb
```

> **Note:** Download `CompleteDataset.csv` from Kaggle and place it in the same directory before running.

---

## 👤 Author

**Anshu** — [GitHub](https://github.com/anshu1516)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
