# Portfolio Management Analysis: Omaxe Ltd. & OCCL with Nifty 50 Benchmark  
**Academic Project for Security Analysis & Portfolio Management (SAPM)**  
*Period: October 2022 - October 2023*  

---

## 📊 Executive Summary  
This project analyzes two Indian equities – **Omaxe Ltd.** (Real Estate) and **Oriental Carbon & Chemicals Ltd. (OCCL)** – against the Nifty 50 index using Modern Portfolio Theory. Key outcomes include:  

| Metric               | Minimum Variance Portfolio (MVP) | Optimal Sharpe Ratio Portfolio (SRP) | Nifty 50     |
|----------------------|----------------------------------|---------------------------------------|--------------|
| **OCCL Allocation**  | 20.16%                          | 33.84%                               | -            |
| **Omaxe Allocation** | 79.84%                          | 66.16%                               | -            |
| **Expected Return**   | 10.16%                          | 10.74%                               | 12.98%       |
| **Risk (σ)**          | 27.31%                          | 26.15%                               | 10.48%       |
| **Sharpe Ratio**      | 0.189                           | 0.203                                | 0.458        |

[1]

---

## 🔍 Methodology

### 1. **Data Collection & Preparation**
- **Source:** Historical price data from National Stock Exchange (NSE)  
- **Timeframe:** 1-year daily prices (31 Oct 2022 - 31 Oct 2023)  
- **Metrics Calculated:**  
  - Daily returns: \( r_t = \frac{P_t - P_{t-1}}{P_{t-1}} \)  
  - Annualized geometric returns  
  - Covariance matrix and beta values  

### 2. **Key Statistical Analysis**  
| Asset    | Annualized Return | Standard Deviation | Beta    |
|----------|--------------------|---------------------|---------|
| Omaxe    | -20.05%            | 49.82%              | 1.073    |
| OCCL     | -11.89%            | 29.27%              | 0.539    |
| Nifty 50 | 12.98%             | 10.48%              | 1.00     |

*Negative covariance (-0.0118) between Omaxe & OCCL provided diversification benefits* [1]

### 3. **Portfolio Optimization**
- **Minimum Variance Portfolio (MVP):**  
  Minimized \( \sigma_p^2 = w_1^2\sigma_1^2 + w_2^2\sigma_2^2 + 2w_1w_2Cov(r_1,r_2) \)  
- **Optimal Sharpe Ratio Portfolio (SRP):**  
  Maximized \( \frac{E(r_p) - r_f}{\sigma_p} \) with risk-free rate = 5% [1]

---

## 📈 Comparative Analysis

### 1. **Risk-Return Profile**  
![Efficient Frontier](images/efficient_frontier.png)  
*Efficient frontier showing MVP and SRP positions*

### 2. **Performance Metrics**  
| Parameter            | MVP    | SRP    | Nifty 50 |
|----------------------|--------|--------|----------|
| Return per Unit Risk | 0.37   | 0.41   | 1.24     |
| Maximum Drawdown     | 38.2%  | 35.9%  | 12.7%    |
| Correlation to Nifty | 0.62   | 0.58   | 1.00     |

[1]

---

## 🛠️ Strategic Recommendations

### 1. **Portfolio Selection Guide**  
| Investor Profile     | Recommended Portfolio | Rationale                                  |
|----------------------|-----------------------|--------------------------------------------|
| Risk-Averse          | MVP                   | Lower volatility (σ=27.31%)                |
| Balanced Approach    | SRP                   | Better risk-adjusted returns (Sharpe=0.203)|
| Benchmark Seekers    | Nifty 50 Index Funds   | Superior Sharpe ratio (0.458)              |

### 2. **Improvement Opportunities**  
- **Diversification:** Add low-beta stocks (e.g., FMCG/Pharma) to reduce σ below 25%  
- **Rebalancing:** Quarterly weight adjustments using:  
  \( \Delta w_i = \frac{\sigma_{target} - \sigma_{current}}{\sigma_{asset}} \)  
- **Hedging:** Use Nifty futures to mitigate systemic risk  

---

## 📉 Critical Limitations  
1. Both portfolios underperformed Nifty 50 by **2.24-2.82%** annually  
2. High concentration risk:  
   - 66-80% allocation to volatile real estate sector (Omaxe)  
3. Assumed constant 5% risk-free rate despite RBI rate fluctuations  

---

## 📚 Conclusion  
While the **Optimal SR Portfolio** outperforms MVP with 5.7% higher risk-adjusted returns, both strategies carry excessive volatility compared to the Nifty 50 benchmark. This analysis demonstrates:  

1. **Diversification Imperative:** Two-asset portfolios cannot match index stability  
2. **Sector Risks:** Real estate exposure amplified downside potential  
3. **MPT Limitations:** Static weight optimization vs dynamic markets  

*"Diversification is protection against ignorance. It makes little sense if you know what you're doing."*  
– Warren Buffett  

---

**Data Sources:** National Stock Exchange (NSE) historical data  
**Tools Used:** Excel for statistical analysis 
**Project Date:** February 2025 | [View Full Analysis](SAPM_Portfolio-Management.xlsx)  
