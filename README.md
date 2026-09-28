# Agribusiness Data Analysis & Price Forecasting 🌾📊

Welcome to my project repository for the **Junior Data Scientist Internship** at **YuvaIntern**. This project focuses on building a reproducible data pipeline to analyze agricultural production, market arrivals, resource utilization, and commodity price trends across India.

## 👤 Intern Information
* **Name:** Priyanshu Kumar Singh
* **Role:** Junior Data Scientist Intern
* **Domain:** Agribusiness Data Analysis
* **Timeline:** September 2026 – October 2026

---

## 🎯 Research Rationale & Scope
Farm-gate and mandi prices in India move sharply within a single season. Supply reacts slowly because crops take months to grow, while weather shocks and festival demand hit within days. Even a modest, honest estimate of where prices are heading gives farmers and traders something better than raw instinct. 

To maintain realistic analytical depth within a five-week schedule, the project scope is restricted to exactly **five key crops**:
* **Perishables (High Volatility):** Tomato, Onion, Potato (TOP)
* **Staples (Regulated/MSP):** Wheat, Rice

---

## 📅 5-Week Roadmap & Deliverables

| Week | Phase | Status | Key Focus & Outputs |
| :---: | :--- | :---: | :--- |
| **Week 1** | **Planning & Strategy** | 🔄 *Current* | Define research rationale, isolate resource metrics, map public data channels, and launch repository framework. |
| **Week 2** | **Data Collection** | ⏳ *Upcoming* | Pull 2–3 years of daily historical mandi data from AGMARKNET and match regional IMD weather/input files. |
| **Week 3** | **Data Cleaning & Merging** | ⏳ *Upcoming* | Address reporting gaps, standardize metrics, and merge datasets across uneven geographic grains. |
| **Week 4** | **Exploratory Data Analysis** | ⏳ *Upcoming* | Execute seasonal decomposition, check market price spreads, and establish a moving-average baseline. |
| **Week 5** | **Predictive Modeling** | ⏳ *Upcoming* | Test ML candidates (Linear Regression, Random Forest, Gradient Boosting) against the baseline to verify forecast lift. |

---

## 📊 Core Variables & Metrics
* **Market Signals:** Daily minimum, modal, maximum prices, and daily arrival volumes (quintals).
* **Supply-Side Signals:** Sown/harvested area, total production volume, and calculated crop yield.
* **Climate Signal:** District-level monthly rainfall and percentage deviation from the long-period average.
* **Resource Utilization:** Share of area under irrigation vs. rain-fed land, and fertilizer intensity per hectare.

---

## 🧮 Planned Analysis Methods (Week 4 Focus)
Before training predictive models, the data will be evaluated using:
1. **Rolling Averages:** To separate long-term pricing trends from day-to-day market noise.
2. **Seasonal Decomposition:** Breaking down price series into structural trend, seasonal cycle, and random residual components.
3. **Lagged Correlation Matrices:** Inspecting how many days it takes for an arrival spike or rainfall deficit to reflect in market prices.
4. **Mandi Price Spreads:** Analyzing variance across different markets to check data consistency and localization flags.

---

## 📁 Repository Structure
```text
├── data/
│   ├── raw/            # Unmodified source files downloaded during Week 2
│   └── processed/      # Cleaned and merged crop tables generated in Week 3
├── notebooks/
│   ├── week3_cleaning.ipynb   # Data preprocessing and standardization logs
│   ├── week4_eda.ipynb        # Seasonal decomposition and correlation analysis
│   └── week5_modeling.ipynb   # Model training, validation, and scoring comparisons
├── README.md           # Project documentation and roadmap (this file)
└── requirements.txt    # Python dependencies for project reproducibility
```

---

## 🌐 Target Open-Data Sources
* **Mandi Prices & Volumes:** [AGMARKNET](https://agmarknet.gov.in) & [e-NAM](https://enam.gov.in)
* **Yield & Input Statistics:** [ES&E Division, Department of Agriculture](https://desagri.gov.in)
* **Meteorological Indicators:** [India Meteorological Department (IMD)](https://imd.gov.in)
