# Global Commodity Market Dynamics: Time-Series Forecasting & Volatility Analysis

An end-to-end quantitative research notebook modeling spot gold price trends ($USD/oz$) and annualized 30-day volatility regimes. This project combines automated data pipelines, Facebook Prophet time-series modeling, and automated macroeconomic narrative synthesis.

---

##  Executive Summary

* **Objective:** Deliver a high-frequency commodity tracking model that pairs 90-day predictive horizons with short-term risk metrics.
* **Pipeline Architecture:** `yfinance` (ETL) $\rightarrow$ `Prophet` (Predictive Modeling) $\rightarrow$ `30-Day Rolling Volatility` (Feature Engineering) $\rightarrow$ `Gemini API` (LLM Executive Briefing).
* **Key Findings:** Identified a moderate trend trajectory alongside compressed annualized volatility, highlighting strategic parameters for sovereign reserve planning and multi-asset risk management.

---

##  Tech Stack & Methodology

* **Data Acquisition:** `yfinance` API pulling historical spot gold prices.
* **Forecasting Engine:** `Prophet` using additive time-series decomposition to capture underlying trend components.
* **Risk Analytics:** 30-day rolling window calculating annualized historical volatility ($\sigma_{annual} = \sigma_{daily} \times \sqrt{252}$).
* **LLM Synthesis:** `google-genai` integration using low-latency prompts to convert raw metrics into structured executive summaries.
* **Visualization:** Minimalist `matplotlib` dual-subplot dashboard.

---

##  Visualizations & Output

The modeling output provides a unified view of both price trajectory and volatility:

1. **Spot Price & 90-Day Forecast:** Historical spot prices paired with a 90-day Prophet forecast and a 95% confidence interval band.
2. **Volatility Regime:** 30-day annualized rolling volatility tracking quiet vs. heightened risk environments.

---

##  How to Run

### 1. Prerequisites
Ensure you have Python 3.10+ installed. Install required dependencies:
```bash
pip install -r requirements.txt
