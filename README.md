# Terry's Trousers — Business Performance & Return Mitigation Simulator

An end-to-end e-commerce data analytics project and interactive strategy modeling tool. This project analyzes unit economics and customer return dynamics for **Terry's Trousers**, identifies key revenue leakage drivers, and provides executive stakeholders with an interactive scenario simulator for strategic decision-making.

🔗 **Live Interactive Simulator:** [https://<your-github-username>.github.io/terrys-trousers-simulator/](https://<your-github-username>.github.io/terrys-trousers-simulator/)

---

## 📌 Executive Summary

Despite generating steady revenue across its apparel lineup, **Terry's Trousers** suffered from high product return rates, significantly eroding net margins through reverse logistics and restocking costs. 

By analyzing sales and return performance across product categories, this project identified that **Baggy Cargos** were responsible for over **55% of all returned units**, driven by a **36% return rate**. An interactive web application was engineered to allow leadership to model target scenarios and evaluate trade-offs between customer acquisition, average order value expansion, and return mitigation.

---

## 📊 Dataset & Baseline Performance

The baseline analysis was conducted on recent transactional sales data (`Trouser Sales Data - Terry's Trousers.csv`) covering **965 orders**.

### Baseline Key Performance Indicators (KPIs)

* **Total Orders:** 965 units
* **Gross Revenue:** $117,025.00
* **Weighted Average Order Value (AOV):** $121.27
* **Overall Return Rate:** 30.26% (292 returned units)
* **Total Direct Return Handling Cost:** $4,172.00
* **Net Revenue (After Returns):** $112,853.00

### Category Performance Breakdown

| Product Category | Orders | AOV ($) | Gross Revenue ($) | Return Rate (%) | Returns (Units) | Cost Per Return ($) | Total Return Cost ($) | Net Revenue ($) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Classic Chinos** | 120 | $85.00 | $10,200.00 | 20.0% | 24 | $12.50 | $300.00 | $9,900.00 |
| **Slim-Fit Denim** | 200 | $110.00 | $22,000.00 | 28.0% | 56 | $14.00 | $784.00 | $21,216.00 |
| **Corduroy Slacks** | 85 | $95.00 | $8,075.00 | 20.0% | 17 | $12.50 | $212.50 | $7,862.50 |
| **Baggy Cargo** | 450 | $140.00 | $63,000.00 | 36.0% | 162 | $15.00 | $2,430.00 | $60,570.00 |
| **Wool Dress Trousers** | 110 | $125.00 | $13,750.00 | 30.0% | 33 | $13.50 | $445.50 | $13,304.50 |
| **TOTAL / AVG** | **965** | **$121.27** | **$117,025.00** | **30.26%** | **292** | **$14.29** | **$4,172.00** | **$112,853.00** |

---

## 🔍 Key Data Insights & Root Cause Analysis

1. **Revenue Concentration Risk:** **Baggy Cargo** represents the largest single product category, driving **53.8% of total gross revenue** ($63,000.00).
2. **Return Rate Disparity:** **Baggy Cargo** exhibits an unsustainable **36.0% return rate**, resulting in **162 returned units** out of 292 total returns across the company (**55.5% of total company returns**).
3. **Logistics Cost Impact:** Direct reverse-logistics handling fees ($15.00/unit for Baggy Cargo) total **$2,430.00** for this category alone, severely diminishing net profits.

---

## 🎯 Strategic Action Plan & Business Levers

Based on data insights, three primary strategic initiatives were established:

1. **Lever 1: Sizing & Fit Optimization (Primary Driver)**
   * *Action:* Deploy an interactive sizing assistant on the product page for loose/baggy fit trousers to address sizing mismatches.
   * *Target:* Reduce Baggy Cargo return rate from 36% to 20%, saving ~97 returned units and ~$1,450 in direct handling costs.
2. **Lever 2: Average Order Value (AOV) Expansion**
   * *Action:* Introduce product bundling (trousers + belts/socks) at checkout.
   * *Target:* Increase weighted AOV from $121.27 to $135.00.
3. **Lever 3: Reverse Logistics Contract Optimization**
   * *Action:* Negotiate volume discounts with third-party logistics (3PL) providers for return shipping labels.
   * *Target:* Lower average cost per return from $14.29 to $11.00.

---

## 💻 Interactive Simulator Tool

To allow executives to dynamically model financial impacts, a client-side web application was engineered using **HTML5, CSS3, and JavaScript**.

### Key Simulator Features
* **Dynamic Sliders:** Allows live adjustment of Average Order Value ($), Return Rate (%), Cost Per Return ($), and Total Order Volume.
* **Real-time Recalculations:** Instantly computes Gross Revenue, Returned Units, Return Costs, and Net Revenue upon slider adjustment.
* **Responsive Dark Dashboard Theme:** Styled with modern CSS grid layouts and custom properties for desktop and mobile visualization.

