# The Economic Cost of Climate Volatility on Indian Agriculture: A District-Level Panel Analysis of Gujarat

## Overview

This project presents a **district-level econometric analysis** of the economic impact of climate volatility on agricultural productivity in Gujarat, India.

Using a **two-way fixed-effects panel regression model**, the study quantifies how rainfall variability and drought shocks affect rice production and translates these effects into **monetary economic losses**.

---

## Key Contributions

* Quantifies **economic cost of climate variability** (not just yield impact)
* Captures **asymmetric effects** of rainfall (drought vs excess rainfall)
* Evaluates effectiveness of **technology inputs (irrigation, fertilizers)**

---

## Dataset

* Custom-built dataset combining multiple sources (ICRISAT, DES, rainfall data)
* Size: ~600 KB
* Observations: **828**
* Features: **117 variables**

### Includes:

* Crop production (rice, wheat)
* Rainfall (monthly & seasonal)
* Fertilizer usage (NPK)
* Irrigation coverage
* Farm Harvest Prices (FHP)
* Agro-climatic indicators (PET)

---

## Project Structure

```id="r9t2kl"
economic-cost-of-climate-volatility/
│
├── data/
│   └── dataset.csv
│
├── notebooks/
│   └── economic-cost-of-climate-volatility.ipynb
│
├── paper/
│   └── research_paper.pdf
│
├── requirements.txt
├── README.md
```

---

## Methodology

### Model Used:

Two-Way Fixed Effects (TWFE) Panel Regression

**Model Specification:**

* Controls for:

  * District-level fixed effects (μᵢ)
  * Time fixed effects (δₜ)
* Clustered standard errors (district-level)

### Key Variables:

* Dependent: Log of rice production
* Climate:

  * Peak monsoon rainfall (July–August)
  * Drought shock indicator
* Controls:

  * Fertilizer consumption (NPK)
  * Net irrigated area

---

## Key Results

### Climate Impact

* **Drought shock → 29.81% drop in rice production**
* Rainfall shows **non-linear (inverse-U) relationship** with output
* Excess rainfall also reduces productivity (flooding, waterlogging)

### Economic Impact

* Total estimated loss:
   **₹139.41 Crores (1966–2011)**

* Losses are highly **regionally concentrated**

  * Highest: Panch Mahals, Kheda

### Technology Insights

* Fertilizers & irrigation:

  * Improve baseline productivity
  * Do NOT significantly reduce climate vulnerability

---

## Key Insights

* Climate volatility has **asymmetric economic effects**
* Agricultural systems remain **highly dependent on monsoon stability**
* Current adaptation strategies are **insufficient at district level**

---

## Policy Implications

* Scale precision irrigation (drip/sprinkler systems)
* Introduce **weather-indexed insurance models**
* Promote **climate-resilient crops** (millets, sorghum)
* Shift from reactive relief → proactive adaptation

---

## Installation & Usage

```id="jv8r2p"
git clone https://github.com/your-username/economic-cost-of-climate-volatility.git
cd economic-cost-of-climate-volatility
pip install -r requirements.txt
jupyter notebook
```

---

## Future Work

* Extend dataset beyond 2011
* Include more crops (cotton, groundnut, wheat)
* Use spatial econometrics for regional spillovers
* Integrate climate model projections (GCMs)

---

<!-- ## Author

Divyansh Jaiswal - 202311030@diu.iiitvadodara.ac.in
K. Hasini Reddy - 202311040@diu.iiitvadodara.ac.in
Rudra Raj Narayan Monas - 202311073@diu.iiitvadodara.ac.in


--- -->