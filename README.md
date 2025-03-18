# Quantitative Market Analysis Project

## Overview
Analyzing systematic relationships between equity indices (S&P, NASDAQ) and commodity/currency markets (gold, oil, copper, natural gas, cattle, FX).

## Folder Structure
- `/data`: Raw market data
- `/notebooks`: Jupyter notebooks with quantitative analysis
- `/scripts`: Python scripts for helper functions
- `/results`: Analysis outputs and visualizations

## Key Analytical Methods:
- Cointegration & correlation analysis
- Granger causality tests
- Regression modeling and scenario simulations

## Tools Used
- Python (`numpy`, `pandas`, `matplotlib`, `statsmodels`, `scipy`, `yfinance`, `scikit-learn`)
- Jupyter Notebooks & VSCode

## Goals
- Clearly define market dynamics and predictive relationships.
- Provide actionable quantitative insights.
- Demonstrate quantitative rigor aligned with Bridgewater’s macro-systematic philosophy.

---

### 🐄 **Strategic Interpretation of Dividend-Adjusted Cattle Returns vs. Equities**

**Explicit Dividend Definition & Context:**  
In this analysis, the revenue explicitly derived from a spring-calving cow-calf operation ($444 per cow annually as per the UKY Agricultural Economics analysis) is treated explicitly as an operational "dividend yield," providing a real-world proxy for consistent annual income. 

To remain explicitly conservative, this analysis **does not include** potentially significant revenue streams from higher-value products such as artisan cheeses, yogurt, and leather goods—revenues which could substantially increase the dividend yield and overall returns.

### 📈 **Risk-Adjusted Return Analysis (Sharpe-like Ratios)**
Comparing cattle farming explicitly adjusted for "operational dividends" against dividend-adjusted returns of major equity indices:

- **Live Cattle Dividend Adjusted Returns** explicitly show consistently superior risk-adjusted returns compared to both the NASDAQ100 and S&P 500, demonstrating:
  - **Higher Annual Returns:** Driven explicitly by stable operational "dividend" yields.
  - **Lower Volatility:** Relative stability explicitly due to the underlying real asset (livestock), as opposed to equities heavily influenced by market sentiment, macroeconomic shocks, and sector rotations.

This comparison suggests explicitly that on a risk-adjusted basis, cattle farming, when structured as a dividend-yielding asset, can significantly outperform equity indices like the S&P500 and NASDAQ100—especially in macroeconomic environments characterized explicitly by volatility, inflation, or uncertainty.

---

### 🧮 **Why Are We Seeing Such Strong Results?**  

- The high explicit operational dividend yield (from annual cow-calf operations) significantly bolsters cumulative returns over time, acting as a powerful compounded growth driver explicitly in stable and inflationary environments.
- The lower explicit volatility for cattle returns (relative to indices) enhances the risk-adjusted attractiveness, clearly highlighting cattle farming’s defensive characteristics explicitly.

---

### 📌 **Implications for Strategic Asset Allocation:**  

- These findings suggest explicitly that large-scale cattle farming operations could serve as a crucial diversifier and hedge explicitly against macroeconomic and inflationary volatility, potentially strengthening long-term risk-adjusted returns in a diversified portfolio.
- Given conservative explicit assumptions (excluding higher-end revenue streams), the true potential for profitability and risk-adjusted outperformance explicitly may be even higher.

---

### 🔑 **Strategic Insights & Final Summary:**

- Explicitly integrating operationally driven dividend-like assets (cattle farming) can significantly enhance portfolio efficiency and returns, particularly in environments where traditional asset yields are suppressed or macroeconomic uncertainty is elevated.
- The analysis explicitly underscores the importance of systematically evaluating real asset investments through a quantitative lens of operational dividends, providing deeper insight explicitly into risk-adjusted returns versus traditional equities.

---

### **📌 Vertical Spread Analysis - README Description**  

#### **Overview**  
The **Vertical Spread Analysis** module is designed to **systematically evaluate short-term, mid-term, and long-term price movements** of NVDA (NVIDIA) stock using **quantitative volatility-based modeling**. This analysis leverages **historical standard deviations, Monte Carlo simulations, and ARIMA forecasting** to identify statistically significant price windows.  

By combining **historical volatility trends** with **forward-looking probabilistic simulations**, this module provides a **structured approach** for identifying **safe entry and exit points** for **vertical spread trading strategies** (credit spreads, debit spreads, and iron condors).  

---

### **🛠️ Methodology**
The **Vertical Spread Analysis** consists of several key components:  

#### **1️⃣ Historical Standard Deviation Analysis**  
- Fetches **historical NVDA price data** from 2015 to present.  
- Computes **rolling standard deviations** over three time horizons:  
  - **Short-Term (21 days) → 1-month window**  
  - **Mid-Term (63 days) → 3-month window**  
  - **Long-Term (252 days) → 1-year window**  
- Defines **price bands** based on ±1σ, ±1.5σ, and ±2σ deviations.  

✅ **Purpose:** This provides insight into expected **price fluctuations** within different time horizons, ensuring traders can structure vertical spreads with **realistic risk levels**.  

---

#### **2️⃣ Monte Carlo Simulations (Next 18 & 8 Weeks)**  
- Runs **1,000 stochastic simulations** to project NVDA’s potential price movements based on **historical returns & volatility**.  
- Ensures **equal standard deviation impact to both upside & downside** for unbiased projections.  
- Filters out **simulations exceeding ±2σ** to maintain **realistic trading zones**.  
- Computes **confidence intervals** for price expectations at multiple risk levels.  

✅ **Purpose:** By modeling a **range of potential price outcomes**, this helps determine the **most probable range** in which NVDA will trade—ideal for defining **strike prices** in vertical spreads.  

---

#### **3️⃣ Short-Term vs. Long-Term Trade Windows**  
- The model is run **twice**, first focusing on **18 months** (long-term positioning) and then on **8 weeks** (short-term tactical trading).  
- Short-term projections help **time spreads effectively within earnings windows**.  
- Long-term projections allow for **structuring safer spreads with better risk-reward ratios**.  

✅ **Purpose:** This enables traders to **customize strategies based on risk tolerance**—whether seeking **high-probability income trades** (credit spreads) or **directional bets on volatility compression** (debit spreads).  

---

### **📊 Key Insights for Trading Vertical Spreads**
- **For Credit Spreads (e.g., Bull Put Spread, Bear Call Spread):**  
  - Ideal to place **short strikes** near **lower/upper ±2σ boundaries** to maximize **premium collection while staying within expected price range**.  
  - Monte Carlo confidence bands help **define high-probability profit zones**.  

- **For Debit Spreads (e.g., Bull Call Spread, Bear Put Spread):**  
  - Best to target **breakouts or mean reversion moves** identified via **historical ±1.5σ levels**.  
  - Avoid opening spreads in **highly volatile conditions** unless supported by historical volatility trends.  

- **For Iron Condors & Butterflies:**  
  - Use **±1.5σ mid-term bands** as reference points for **defining range-bound strategies**.  
  - **Low-volatility environments** (narrow ±1σ range) → Favor **iron condors**.  
  - **High-volatility environments** (wide ±2σ range) → Favor **wider butterflies**.  

---

### **💡 Why This Matters for Traders**  
✅ **Systematic risk assessment:** Reduces subjectivity in choosing **spread strike prices**.  
✅ **Statistical edge:** Combines **historical & probabilistic methods** to guide trade structure.  
✅ **Tactical flexibility:** Adapt strategies for **both short-term & long-term volatility conditions**.  
✅ **Improved probability of success:** Aligns spread risk with **realistic price expectations** instead of speculation.  

---

### **🚀 Next Steps**
📌 **Enhancements planned:**  
- Incorporate **IV Rank & Implied Volatility modeling** to refine entry points.  
- Add **Options Delta Hedging simulations** for optimizing spread adjustments.  
- Expand Monte Carlo to **3,000+ runs** for higher statistical robustness.  

📌 **How to Use This Analysis:**  
- Run **18-month model** for **macro trend trading & LEAPS-based vertical spreads**.  
- Run **8-week model** for **earnings-driven trades & weekly/monthly options spreads**.  
- Combine **both insights** to optimize **spread placement & risk management**.  

