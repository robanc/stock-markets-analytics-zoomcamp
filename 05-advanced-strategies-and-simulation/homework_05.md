# Stock Markets Analytics Zoomcamp 2026 — Module 5 Homework

## Question 1 — 5G Network Investment and Telecom Equipment Stocks

### 1. Market and scope
I would study Nokia (NOK) and Ericsson (ERIC), using their U.S.-listed shares, with emphasis on U.S. mobile-network investment by T-Mobile, AT&T, and Verizon. My intended investment horizon is **3–12 months**, using quarterly information.

### 2. Investment thesis
My hypothesis is that **unexpected increases** in carrier spending on 5G Standalone, radio access networks, packet-core modernization, and capacity expansion may predict higher equipment-supplier orders or revenue over the next one to three quarters. The potential stock signal is not 5G growth alone, but spending that exceeds previously communicated expectations and is relevant to a particular supplier. I would test whether this predicts supplier revenue surprises and 3-, 6-, or 12-month subsequent returns.

### 3. Potential edge
My experience with packet-core engineering, SMF/UPF deployments, integration, and capacity planning may help me interpret public technical announcements. A software upgrade, capacity expansion, and major equipment procurement have different implications for supplier revenue. I would use **only public information**, distinguishing operational activity from actual purchase commitments and reported sales.

### 4. Data and sources
**Public source locations identified (not yet a verified historical dataset):** Nokia annual reports and quarterly results; Ericsson annual reports and quarterly results; FCC National Broadband Map / Broadband Data Collection. These respectively report supplier financial performance and mobile coverage. FCC coverage is an indirect deployment indicator, **not** a measure of equipment purchases.

**Still to verify and collect:** quarterly carrier capital expenditures and guidance, with original release dates, from T-Mobile, AT&T, and Verizon investor-relations filings; supplier contract announcements and geographic exposure; adjusted daily NOK/ERIC prices and dividends; historical expectations or guidance needed to define a spending *surprise*; and any licensed industry spending estimates. The historical coverage and point-in-time availability of these data remain to be assessed.

### 5. Research approach
I would build a quarterly **5G Investment Momentum Score** from year-over-year carrier capital-expenditure changes, revisions to published guidance, and publicly reported deployment activity. Supplier-specific exposure would determine whether a signal applies to NOK or ERIC. I would first test whether the score predicts next-quarter-to-three-quarter supplier sales growth or revenue surprises using a simple regression, then test whether it predicts 3-, 6-, and 12-month returns. A provisional trading rule would hold the exposed supplier only when the score exceeds a prespecified threshold; otherwise it would hold cash or short-term Treasuries. Every feature would be timestamped to its public release date to avoid look-ahead bias.

### 6. Validation and risks
I would compare the strategy with buy-and-hold NOK, buy-and-hold ERIC, an equal-weight supplier portfolio, and a broad-market benchmark. I would assess forecast error, cumulative and risk-adjusted returns, drawdown, and results after trading costs. I would reject the thesis if predictive improvement does not survive chronological out-of-sample testing, if returns are explained by existing supplier guidance or market momentum, or if the apparent advantage disappears after costs. Key risks are delayed reporting, global supplier revenue exposure, carrier-to-supplier contract uncertainty, foreign exchange, shifting supplier market share, and the possibility that public announcements are already priced in.

**Research links:** [Nokia annual reports](https://www.nokia.com/about-us/investors/results-reports/annual-report/); [Ericsson annual reports](https://www.ericsson.com/en/investors/financial-reports-and-presentations/annual-reports); [FCC National Broadband Map](https://broadbandmap.fcc.gov/).

---

## Question 2 — NVIDIA–AMD Semiconductor Pairs Trading

### 1. Market and scope
I would investigate the NASDAQ-listed shares of NVIDIA (NVDA) and Advanced Micro Devices (AMD), which both participate in GPU and data-center computing markets but have different product mixes and competitive positions. The intended holding period is **5–20 trading days**.

### 2. Investment thesis
Broad semiconductor and AI-infrastructure news can affect both companies, while company-specific announcements can cause their prices to diverge. My testable hypothesis is that **some unusually large deviations from a stable, estimated relative-price relationship** subsequently converge within 5–20 trading days. This only makes sense if a stable relationship exists; a persistent divergence may instead reflect real changes in competition or earnings expectations.

### 3. Potential edge
Rather than forecast the direction of semiconductor stocks, I would seek short-lived relative mispricing. I would combine statistical tests with a review of public earnings, product, and regulatory news to distinguish temporary dislocations from structural breaks. The edge is hypothetical and must be demonstrated after short-selling costs.

### 4. Data and sources
**Public source locations identified (not yet a verified historical dataset):** NVIDIA and AMD investor-relations filings for earnings, business segments, and announcement dates; published academic literature on cointegration and pairs trading.

**Still to verify and collect:** split- and dividend-adjusted daily prices, volumes, borrowing costs and short availability; point-in-time earnings dates; a semiconductor benchmark such as SMH; and a sufficiently long historical sample, tentatively 2018–2026. Historical price adjustments, data-provider terms, and point-in-time event dates need verification.

### 5. Research approach
I would calculate rolling return correlation, then test log prices for cointegration on a **training window**. If a stable relationship is supported, I would estimate a hedge ratio and the spread, then calculate a rolling spread z-score using only past data. A provisional rule is to open a hedged long/short position when the z-score exceeds **+2** or falls below **−2**, close when it approaches zero, and impose a **20-trading-day maximum hold**. The exact direction and share quantities would follow the estimated spread and hedge ratio. I would re-estimate parameters on rolling historical windows and stop trading when relationship-stability tests fail.

### 6. Validation and risks
I would compare net performance with a cash/no-trade baseline, an equal-weight NVDA–AMD buy-and-hold portfolio, and SMH. Metrics would include net return, Sharpe ratio, maximum drawdown, win rate, and holding period. I would reject the pair if cointegration is unstable, out-of-sample convergence is unreliable, or profits vanish after bid–ask spread, slippage, borrow fees, and financing costs. Major risks include changing AI market share, earnings gaps, export controls, extreme valuation changes, and potentially unbounded losses on short positions. Correlation alone would not justify a trade.

**Research links:** [NVIDIA annual reports](https://investor.nvidia.com/financial-info/annual-reports-and-proxies/default.aspx); [AMD investor relations](https://ir.amd.com/); [VanEck SMH](https://www.vaneck.com/us/en/investments/semiconductor-etf-smh/).

---

## Question 3 — AI Data Center Infrastructure Demand and Supplier Stocks

### 1. Market and scope
I would study NYSE-listed Vertiv (VRT) and Eaton (ETN), suppliers of data-center power, electrical distribution, and cooling-related infrastructure. The primary market focus would be U.S. hyperscale data-center expansion. My intended investment horizon is **3–12 months**, evaluated quarterly.

### 2. Investment thesis
AI computing increases demand for electricity delivery, backup power, and thermal management. My hypothesis is that **upward surprises in hyperscaler capital-spending guidance**, when linked to data-center capacity expansion, may predict stronger future supplier orders, backlog conversion, revenue surprises, and subsequent stock returns over one to four quarters. Higher spending does not guarantee higher returns: what matters is unexpected, supplier-relevant demand beyond current market expectations.

### 3. Potential edge
My background in network capacity planning, equipment integration, and infrastructure rollout could help me distinguish an announced data-center project from a project approaching actual equipment procurement and installation. I would focus on timing and bottlenecks—power connections, cooling requirements, equipment lead times, and backlog conversion—using public sources rather than treating every AI investment headline as an immediate sales signal.

### 4. Data and sources
**Public source locations identified (not yet a verified historical dataset):** Microsoft annual reports for infrastructure investment disclosures; Vertiv and Eaton investor-relations reports for revenue, orders, backlog, and business outlook; U.S. Energy Information Administration publications for electricity-demand context. EIA forecasts are **not** direct measures of equipment orders.

**Still to verify and collect:** quarterly capex and guidance from Microsoft, Amazon, Alphabet, and Meta, with publication timestamps; comparable quarterly VRT/ETN order and backlog series; analyst revenue expectations available before earnings; adjusted historical prices and dividends; and project-level data on construction, interconnection, and commissioning. Hyperscaler capex also includes GPUs, buildings, and networking, so only part is addressable by these suppliers.

### 5. Research approach
I would construct a quarterly **AI Infrastructure Demand Momentum Score** from revisions to hyperscaler capex guidance, growth in disclosed infrastructure investment, and independently reported expansion or power-capacity constraints. I would first test whether this score predicts VRT/ETN order growth and revenue surprises over the next one to four quarters, controlling for previously disclosed supplier backlog and prior sales growth. Next, I would evaluate 3-, 6-, and 12-month subsequent stock returns. A provisional trading rule would buy a supplier when the score exceeds a predetermined threshold and public disclosures support meaningful exposure; otherwise it would hold cash or short-term Treasuries. All inputs would be aligned to when investors could actually observe them.

### 6. Validation and risks
I would compare forecast performance with simple historical-sales and prior-backlog baselines, and trading performance with buy-and-hold VRT, buy-and-hold ETN, an equal-weight portfolio, and the S&P 500. I would assess forecast errors, cumulative and risk-adjusted returns, maximum drawdown, and transaction costs. I would reject the thesis if the score adds no out-of-sample predictive value beyond backlog or guidance, or if excess returns vanish after costs. Risks include already-high valuations, power and permitting delays, order cancellations, inconsistent backlog definitions, supplier business-mix differences, capex not flowing to these vendors, and limited quarterly observations.

**Research links:** [Microsoft annual reports](https://www.microsoft.com/investor/reports/ar26/); [Vertiv investor relations](https://investors.vertiv.com/overview/default.aspx); [Eaton investor relations](https://www.eaton.com/us/en-us/company/investor-relations.html); [EIA](https://www.eia.gov/).

---

*Status: Three exploratory research proposals. No datasets have been downloaded or independently backtested for this homework. Source links identify where the proposed data can be investigated; historical completeness, licensing, and publication timing require verification before implementation.*
