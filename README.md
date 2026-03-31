# 🏥 NHS GP Appointment Efficiency Analysis | Python & Data Analytics

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python) ![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-lightblue) ![Seaborn](https://img.shields.io/badge/Seaborn-Visualisation-orange) ![Matplotlib](https://img.shields.io/badge/Matplotlib-Plotting-green) ![LSE](https://img.shields.io/badge/LSE-DA201-red) ![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)

> **LSE Data Analytics using Python | DA201**
> Diagnostic Analysis of NHS Appointment Efficiency — August 2021 to June 2022

---

## 📌 Project Overview

This project was completed as a graded assignment for the **LSE Data Analytics using Python (DA201)** programme.

The National Health Service (NHS) faces a persistent operational challenge from missed GP appointments — formally classified as DNA (Did Not Attend) events. This analysis addresses two core mandates:

1. **Mandate 1** — Were adequate staff and capacity available within NHS networks?
2. **Mandate 2** — How effectively were available resources being utilised?

Using Python and four NHS-published datasets comprising **817,000+ records**, the analysis uncovers capacity trends, DNA patterns, booking behaviour, appointment modes, and social media sentiment — delivering **7 evidence-based recommendations** to improve NHS appointment efficiency.

---

## 📁 Repository Structure
```
NHS-GP-Appointment-Analysis-LSE/
│
├── data/
│   ├── actual_duration.csv          # Appointment duration by sub-ICB location
│   ├── national_categories.xlsx     # National categories & service settings
│   └── tweets.csv                   # NHS-related Twitter/X dataset
│
├── notebooks/
│   └── LSE_TP_DA201_Assignment_Final.ipynb   # Main analysis notebook
│
├── report/
│   └── NHS_Diagnostic_Analysis_Report.pdf    # Full technical report
│
├── images/                          # Exported visualisations
│
└── README.md
```

---

## 📊 Datasets

| Alias | File | Key Variables | Rows | Date Range |
|-------|------|--------------|------|------------|
| AD | actual_duration.csv | Location, date, duration, count | 137,793 | Dec 2021–Jun 2022 |
| AR | appointments_regional.csv | Status, HCP type, mode, booking lead time | 596,821 | Jan 2020–Jun 2022 |
| NC | national_categories.xlsx | Service setting, context type, nat. category | 817,394 | Aug 2021–Jun 2022 |
| TW | tweets.csv | Tweet text, hashtags, retweet/fav counts | 1,174 | N/A |

> Data sourced from NHS England open data. All datasets contained zero missing values and zero duplicate records.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Python 3.x** | Core programming language |
| **Pandas** | Data loading, cleaning, transformation, groupby aggregations |
| **Seaborn** | Statistical visualisations |
| **Matplotlib** | Custom plots and chart formatting |
| **NumPy** | Numerical computations |
| **Jupyter Notebook** | Interactive development environment |

---

## 🔍 Key Findings

### Mandate 1 — Capacity & Staffing
- NHS national capacity **(1.2M appointments/day) was never breached** during Aug 2021–Jun 2022
- **Peak utilisation: 84.5%** in November 2021 (daily avg: 1,013,502 appointments)
- **Period average: 74.8%** — ~25% headroom maintained throughout
- **Busiest month:** November 2021 with **30.4M appointments**
- A blanket national staffing increase is **not supported** by the aggregate data

### Mandate 2 — Resource Utilisation
- **DNA events** spiked to **1,565,624 in October 2021** — directly correlating with peak demand months
- **44.2% of bookings were Same Day**, confirming the reactive nature of NHS primary care
- **Face-to-Face appointments dominate at 62%**; Video/Online consistently underutilised
- GP and Other Practice Staff followed near-identical seasonal patterns — confirming **demand, not staffing**, drives variation
- Twitter/X hashtag analysis of 1,174 tweets revealed growing public discourse around **#AI** and **#digitalhealth**

---

## 💡 Recommendations

1. **Do not broadly increase staffing** — investigate sub-ICB and seasonal hotspots first
2. **Proactively reduce DNA appointments** — deploy SMS, email & Twitter/X campaigns 2–4 weeks ahead of Oct–Nov peaks
3. **Pilot extended weekend access** — to smooth Monday bottlenecks
4. **Promote telephone and video appointments** — reduce face-to-face congestion at no additional staffing cost
5. **Monitor 8–28 day booking lead times** — rising advance bookings signal same-day slot exhaustion
6. **Use Twitter/X strategically** — #healthcare (769 occurrences) provides a direct public engagement channel
7. **Accelerate NHS data standardisation** — continue NHS-wide standardisation for better analytical decision-making

---

## ▶️ How to Run
```bash
# 1. Clone the repository
git clone https://github.com/yourusername/NHS-GP-Appointment-Analysis-LSE.git

# 2. Navigate to the project directory
cd NHS-GP-Appointment-Analysis-LSE

# 3. Install dependencies
pip install pandas numpy matplotlib seaborn openpyxl jupyter

# 4. Launch Jupyter Notebook
jupyter notebook notebooks/LSE_TP_DA201_Assignment_Final.ipynb
```

---

## 👩‍💻 Author

**Vaishnavi Mishra**
LSE Data Analytics using Python | DA201
[LinkedIn](https://www.linkedin.com/in/yourprofile) | [GitHub](https://github.com/yourusername)
```
