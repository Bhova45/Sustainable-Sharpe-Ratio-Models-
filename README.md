
# 🌟 Sustainable Sharpe Ratio Models

## 💡 Project Overview

This repository contains the analysis and implementation of the **Sustainable Sharpe Ratio (SSR)**, a critical modification of the traditional Sharpe Ratio designed to incorporate **Environmental, Social, and Governance (ESG)** factors into the risk-adjusted performance evaluation of investment portfolios.

The core goal of this project is to develop and test models that balance financial return maximization with sustainability objectives, providing a more holistic view of portfolio performance.

## 💾 Repository Contents

The main analysis is contained within the following Jupyter Notebook:

* `Sustainable Sharpe Ratio Models.ipynb`: The primary notebook detailing data acquisition, methodology, model implementation, and comparative results between the Standard Sharpe Ratio (SR) and the Sustainable Sharpe Ratio (SSR).

## 📐 Methodology Highlights

The notebook covers the following key stages:

1.  **Data Acquisition:** Fetching historical stock prices and integrating them with corresponding ESG rating datasets.
2.  **Return Calculation:** Standardizing data and calculating daily/annualized returns.
3.  **SSR Definition:** Defining the mathematical framework for the SSR (e.g., how ESG scores are used to adjust volatility or returns).
4.  **Model Implementation:** Creating Python functions for both standard SR and the custom SSR.
5.  **Portfolio Optimization:** Utilizing techniques (such as Monte Carlo simulations) to determine the optimal portfolio weights under both the SR and SSR criteria, resulting in a comparison of two distinct "Efficient Frontiers."

### The Sustainable Sharpe Ratio (SSR)

The SSR metric used in this analysis is defined as:

$$SSR = \frac{E[R_p - R_f]}{\sigma_{p, adj}}$$

*Where $\sigma_{p, adj}$ is the **adjusted portfolio volatility**, which is penalized or weighted based on the portfolio's aggregate ESG score.*

## 📊 Key Findings

* **Trade-off Observation:** The analysis demonstrates a tangible trade-off where portfolios optimized for a higher SSR often exhibit lower conventional volatility but may differ significantly from portfolios optimized purely for the maximum standard SR.
* **Impact of ESG:** The notebook visualizes how the incorporation of ESG data shifts the position and shape of the Efficient Frontier, providing actionable insights for sustainable investing.

## 🤝 Contribution

Feel free to open issues, submit bug reports, or propose enhancements via pull requests. All feedback is welcome!
