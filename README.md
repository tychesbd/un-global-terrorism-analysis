# 🌍 United Nation Global Terrorism Analysis
### Exploratory Data Analysis | Capstone Project

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?style=flat&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12+-4C8CBF?style=flat)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7+-11557c?style=flat)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat&logo=jupyter&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=flat)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat)

---

## 📌 Project Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on the **Global Terrorism Database (GTD)** — one of the most extensive open-source datasets of terrorist incidents in the world. Covering **181,691 attacks across 205 countries from 1970 to 2017**, the analysis uncovers temporal trends, geographic hotspots, attack patterns, weapon lethality, and organizational activity to generate actionable intelligence for global security policymakers.

The analysis follows the academic **UBM Rule** — Univariate → Bivariate → Multivariate — and produces **15 professional visualizations** with full interpretations, hypothesis testing, statistical analysis, and policy recommendations.

---

## 🗂️ Table of Contents

- [Project Overview](#-project-overview)
- [Dataset](#-dataset)
- [Project Architecture](#-project-architecture)
- [Key Questions Answered](#-key-questions-answered)
- [Hypotheses Tested](#-hypotheses-tested)
- [Visualizations](#-visualizations)
- [Key Findings](#-key-findings)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [How to Run](#-how-to-run)
- [Rubric Coverage](#-rubric-coverage)
- [Limitations](#-limitations)
- [Future Scope](#-future-scope)
- [Author](#-author)

---

## 📊 Dataset

| Attribute | Details |
|---|---|
| **Source** | Global Terrorism Database (GTD) — START, University of Maryland |
| **Time Span** | 1970 – 2017 (47 years) |
| **Total Records** | ~181,691 terrorist incidents |
| **Total Features** | 135 columns |
| **File Name** | `globalterrorismdb_0718dist.csv` |
| **Encoding** | Latin-1 |
| **Size** | ~150 MB |

### Key Columns Used

| Column | Description |
|---|---|
| `iyear` | Year of the incident |
| `country_txt` | Country where the attack occurred |
| `region_txt` | World region (12 categories) |
| `attacktype1_txt` | Type of attack (bombing, assault, etc.) |
| `weaptype1_txt` | Weapon used |
| `targtype1_txt` | Target category (civilian, government, etc.) |
| `gname` | Name of the terrorist organization |
| `nkill` | Number of fatalities |
| `nwound` | Number of wounded |
| `claimed` | Whether responsibility was claimed |
| `suicide` | Whether it was a suicide attack |
| `success` | Whether the attack succeeded |

> ⚠️ The dataset is **not included** in this repository due to its large size. Download it from [Kaggle — Global Terrorism Database](https://www.kaggle.com/datasets/START-UMD/gtd) and place the CSV in the root project directory.

---

## 🏗️ Project Architecture

```
Project Statement Understanding
        │
        ▼
  Hypotheses & Assumptions
  (8 testable hypotheses)
        │
        ▼
     Visualizations
  (UBM Rule — 15 Charts)
        │
        ▼
   Drawing Insights
   (Policy Recommendations)
        │
        ▼
      Conclusion
```

---

## ❓ Key Questions Answered

1. How has global terrorism evolved over the 1970–2017 period?
2. Which countries and regions are most severely affected?
3. What attack types and weapons are most commonly used — and most lethal?
4. Which terrorist organizations are the most active?
5. Are claimed attacks more deadly than unclaimed ones?
6. What types of targets are attacked most frequently?
7. Is there a correlation between suicide attacks and higher fatality rates?
8. How have regional terrorism trends diverged across decades?

---

## 🧪 Hypotheses Tested

| # | Hypothesis | Verdict |
|---|---|---|
| H1 | Terrorist attacks increased significantly after 2001 | ✅ Confirmed |
| H2 | Middle East & North Africa is the most targeted region | ✅ Confirmed |
| H3 | Bombing/Explosion is the most common attack type | ✅ Confirmed |
| H4 | Bombings cause the highest average fatalities per attack | ✅ Partially Confirmed |
| H5 | Private Citizens & Property are the most common target | ✅ Confirmed |
| H6 | Taliban and ISIL are among the most active groups post-2000 | ✅ Confirmed |
| H7 | Unclaimed attacks result in fewer casualties | ✅ Partially Confirmed |
| H8 | Iraq is the single most attacked country | ✅ Confirmed |

---

## 📈 Visualizations

The notebook contains **15 charts** organized by the UBM Rule:

### 🔵 Univariate Analysis
| Chart | Type | Description |
|---|---|---|
| Chart 1 | Line / Area | Terrorist attacks per year (1970–2017) with key event markers |
| Chart 2 | Horizontal Bar | Distribution of attack types |
| Chart 3 | Horizontal Bar | Total attacks by world region |
| Chart 4 | Vertical Bar | Top 10 most attacked countries |
| Chart 5 | Histogram + Box Plot | Distribution of fatalities per attack |

### 🟢 Bivariate Analysis
| Chart | Type | Description |
|---|---|---|
| Chart 6 | Horizontal Bar | Average fatalities by attack type |
| Chart 7 | Horizontal Bar | Total fatalities by region (in thousands) |
| Chart 8 | Horizontal Bar | Top 15 most active terrorist organizations |
| Chart 9 | Multi-line | Attack trends by top 5 regions over time |
| Chart 10 | Dual-axis Bar + Line | Target type — attack frequency vs. avg fatalities |
| Chart 11 | Box Plot + Bar | Claimed vs. unclaimed attacks — casualty comparison |
| Chart 12 | Horizontal Bar | Weapon type vs. total and avg fatalities |

### 🔴 Multivariate Analysis
| Chart | Type | Description |
|---|---|---|
| Chart 13 | Heatmap | Attacks matrix — Region × Decade |
| Chart 14 | Correlation Heatmap | Pearson correlation among numerical variables |
| Chart 15 | Pair Plot | All pairwise relationships (sampled, n=5,000) |

---

## 🔑 Key Findings

- **Post-2001 surge**: Terrorism attacks more than tripled after 2001, peaking in 2014–2016 during ISIL's territorial expansion.
- **MENA dominates**: The Middle East & North Africa accounts for ~25–28% of all global attacks and the highest total fatalities.
- **Iraq leads all nations**: With 24,000+ incidents, Iraq records nearly twice as many attacks as the second-ranked country.
- **Explosives are king**: Bombing/Explosion represents 45%+ of all attacks and the highest aggregate death toll.
- **Taliban & ISIL**: The two most prolific terrorist organizations in the modern era by attack count.
- **Soft targets preferred**: Private citizens & property is the most frequently targeted category globally.
- **Suicide = more lethal**: Suicide attacks show a clear positive correlation with higher fatality counts.
- **Regional divergence**: South America and Western Europe have dramatically reduced terrorism since their 1980s–90s peaks, demonstrating that evidence-based policy works.

---

## 🛠️ Tech Stack

| Library | Version | Purpose |
|---|---|---|
| `Python` | 3.10+ | Core language |
| `pandas` | 2.0+ | Data manipulation and aggregation |
| `numpy` | 1.24+ | Numerical operations |
| `matplotlib` | 3.7+ | Core plotting and formatting |
| `seaborn` | 0.12+ | Statistical visualizations |
| `Jupyter Notebook` | 6.5+ | Interactive development environment |

---

## 📁 Project Structure

```
un-global-terrorism-eda/
│
├── 📓 UN_Global_Terrorism_EDA.ipynb    ← Main analysis notebook
├── 📄 README.md                         ← This file
├── 📄 requirements.txt                  ← Python dependencies
│
├── 📂 data/                             ← (gitignored — download separately)
│   └── globalterrorismdb_0718dist.csv
│
└── 📂 assets/                           ← (optional) exported chart images
    ├── chart_01_attacks_per_year.png
    ├── chart_02_attack_types.png
    └── ...
```

---

## ▶️ How to Run

### Option A — Google Colab (Recommended)

1. Open [Google Colab](https://colab.research.google.com/)
2. Upload `UN_Global_Terrorism_EDA.ipynb`
3. Upload the dataset CSV to the Colab session storage:
   ```python
   from google.colab import files
   files.upload()  # select globalterrorismdb_0718dist.csv
   ```
4. Click **Runtime → Run All**

### Option B — Local Jupyter Notebook

**1. Clone the repository**
```bash
git clone https://github.com/your-username/un-global-terrorism-eda.git
cd un-global-terrorism-eda
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Add the dataset**
```
Place globalterrorismdb_0718dist.csv in the project root directory.
```

**4. Launch Jupyter**
```bash
jupyter notebook UN_Global_Terrorism_EDA.ipynb
```

**5. Run all cells**
```
Kernel → Restart & Run All
```

### requirements.txt
```
pandas>=2.0.0
numpy>=1.24.0
matplotlib>=3.7.0
seaborn>=0.12.0
jupyter>=1.0.0
notebook>=6.5.0
```

---

## ✅ Rubric Coverage

| Rubric Item | Status |
|---|---|
| Summary and Technical Documentation | ✅ 500–600 word project summary included |
| Exploration — Head, Tail, Summary, Data Dictionary | ✅ Full section with annotated code |
| Handling NaN / Null / Missing Values | ✅ Logic documented per column |
| Correlation, Trends, Conclusions from Data | ✅ Correlation heatmap + trend analysis |
| Milestones from Problem Statement | ✅ All 8 hypotheses tested and concluded |
| At Least 5 Different Visualization Types | ✅ 15 charts — 7+ distinct chart types |
| Final Summary of Conclusion | ✅ Dedicated conclusion section |
| Commented Code | ✅ Every code block is fully commented |
| Proper Output Formatting | ✅ Consistent styling, labels, and titles |
| Modularity of Code | ✅ Logical section separation throughout |

---

## ⚠️ Limitations

- **Attribution gap**: Over 40% of attacks are attributed to 'Unknown' groups — a significant intelligence gap in the data.
- **Reporting bias**: Incidents in conflict zones with limited media access may be systematically underreported.
- **Casualty completeness**: ~40% of incidents have missing casualty counts; zero-filled per GTD convention.
- **Definition edge cases**: Borderline cases between state violence and terrorism may introduce classification inconsistencies.
- **Dataset currency**: Ends at 2017 — post-ISIL fragmentation and recent terrorism trends (2018–present) are not captured.

---

## 🔭 Future Scope

1. **Predictive Modeling** — Apply ML (Random Forest, XGBoost) to predict attack likelihood and severity.
2. **NLP / Text Mining** — Extract thematic intelligence from `summary` and `motive` text columns.
3. **Economic Correlation** — Join GTD with GDP, HDI, and Conflict Index data to analyze root causes.
4. **Network Analysis** — Map terrorist group collaboration, splintering, and ideological evolution over time.
5. **Interactive Dashboard** — Build a Plotly/Dash or Power BI dashboard for real-time drill-down exploration.
6. **Dataset Extension** — Update with post-2017 data from GTD's latest releases to track current trends.

---

## 👤 Author

**[Shiv Bijay Deep]**
- 📧 Email: tychesbd@gmail.com
- 🔗 LinkedIn: [linkedin.com/in/shivbijaydeep](https://linkedin.com/in/yourprofile)
- 🐙 GitHub: [github.com/tychesbd](https://github.com/tychesbd)

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements


- **Alma Better** — for making the dataset publicly accessible.


---

> *"Data is the new intelligence. Understanding terrorism through data is the first step toward preventing it."*
