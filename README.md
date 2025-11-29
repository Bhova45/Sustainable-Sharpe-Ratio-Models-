# The Sustainable Sharpe Ratio (SSR): Optimizing ESG-Compliant Portfolio Performance 🌍📈

This repository contains the analysis and implementation of the **Sustainable Sharpe Ratio (SSR)**, a critical modification of the traditional Sharpe Ratio. The SSR is designed to incorporate **Environmental, Social, and Governance (ESG) factors**—specifically Carbon Exposure—into the risk-adjusted performance evaluation of investment portfolios.

The core goal of this project is to develop and test models that balance financial return maximization with strict sustainability objectives (e.g., EU SFDR compliance), providing a more holistic view of portfolio performance for global asset managers.

---

### 💾 Repository Contents

The main analysis is contained within the following Jupyter Notebook:

* **Sustainable Sharpe Ratio Models.ipynb:** The primary notebook detailing data acquisition, methodology, model implementation, and comparative results between the Standard Sharpe Ratio (SR) and the custom Sustainable Sharpe Ratio (SSR).

**Data Sources:** Historical pricing from **Yahoo! Finance**, Risk-Free Rate (DGS10) from **FRED**, and custom Sector/Industry mapping for the **GHG Penalty Factor**.

---

### 📐 Methodology Highlights

The notebook covers the following key stages:

1.  **Data Acquisition:** Fetching historical stock prices and integrating them with corresponding ESG (Carbon Exposure) datasets.
2.  **Return Calculation:** Standardizing data and calculating daily/annualized returns.
3.  **SSR Definition:** Defining the mathematical framework for the SSR, as detailed below.
4.  **Model Implementation:** Creating Python functions for both standard SR and the custom SSR.
5.  **Portfolio Optimization:** Utilizing techniques (such as Monte Carlo simulations) to determine the optimal portfolio weights under both SR and SSR criteria, resulting in a comparison of two distinct **"Efficient Frontiers."**

#### The Sustainable Sharpe Ratio (SSR)

The SSR metric used in this analysis is defined as:

$$\text{SSR} = \frac{E[R_p - R_f]}{\sigma_{p, adj}}$$

Where $\sigma_{p, adj}$ is the **adjusted portfolio volatility**. The mathematical framework defines this adjusted volatility as the standard volatility penalized by the **portfolio's aggregate Carbon Exposure Score (CES)**. This score is derived from industry-specific GHG intensity (or similar ESG data), effectively increasing the perceived risk for non-compliant assets.

---

### 📊 Key Findings

* **Trade-off Observation:** The analysis demonstrates a tangible **trade-off** where portfolios optimized for a higher SSR often exhibit lower conventional volatility but may deliver slightly lower gross returns compared to purely financial-driven portfolios.
* **Impact of ESG on Risk:** The notebook visualizes how incorporating the SSR metric forces the **Efficient Frontier** to **shift inward and to the left** , demonstrating the cost of sustainability, while providing a clear set of optimal portfolios that satisfy dual mandates (financial and ESG compliance).
* **Metric Validation:** The SSR successfully screens out investments facing high Principal Adverse Impact (PAI) risks, proving its value as a compliant financial selection tool.

---

### 🤝 Contribution

Feel free to open issues, submit bug reports, or propose enhancements via pull requests. All feedback is welcome!

