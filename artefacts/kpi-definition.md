# KPI Definition Document

## Project Information

| Field | Details |
|---|---|
| **Project** | Frutilicious Café Analytics Solution |
| **Business Analyst** | Ved Redkar \| Visionize Consultancy LLP |
| **Version** | 1.0 |

---

# KPI Framework Overview

The following KPIs were defined through stakeholder elicitation sessions with the café owner. Each KPI was selected based on the owner's stated business objectives:

- Reducing inventory wastage  
- Understanding sales performance  
- Making faster daily operational decisions  
- Reducing reliance on memory and manual counting  

---

# KPI-001: Daily Gross Revenue

| Field | Detail |
|---|---|
| **Definition** | Total revenue generated from all menu item sales in a single day before any deductions |
| **Formula** | Σ (Units Sold per Item × Unit Price per Item) |

:contentReference[oaicite:0]{index=0}

| **Data Source** | Excel sales log — quantity and price columns |
| **Frequency** | Daily |
| **Target** | Owner-defined weekly revenue goal ÷ 7 |

:contentReference[oaicite:1]{index=1}

| **Threshold — Green** | ≥ Daily target |
| **Threshold — Amber** | 80–99% of daily target |
| **Threshold — Red** | < 80% of daily target |
| **Business Objective** | Track income generation and identify low revenue days early |

---

# KPI-002: Inventory Wastage Percentage

| Field | Detail |
|---|---|
| **Definition** | Proportion of total stock consumed that was wasted rather than sold |
| **Formula** | (Total Wastage Quantity ÷ Total Stock Used) × 100 |

:contentReference[oaicite:2]{index=2}

| **Data Source** | Excel wastage log column |
| **Frequency** | Weekly |
| **Target** | < 10% wastage rate per week |
| **Threshold — Green** | < 10% |
| **Threshold — Amber** | 10–15% |
| **Threshold — Red** | > 15% |
| **Business Objective** | Directly measure and reduce the inventory wastage problem that initiated the engagement |
| **Baseline** | Pre-solution wastage estimated at ~25% |
| **Post-Solution Target** | < 10% |

---

# KPI-003: Stock Depletion Rate

| Field | Detail |
|---|---|
| **Definition** | Average daily consumption rate of each ingredient, used to project stockout dates |
| **Formula** | Total Units Consumed over Period ÷ Number of Days in Period |

:contentReference[oaicite:3]{index=3}

| **Data Source** | Excel inventory log — opening stock, closing stock, wastage |
| **Frequency** | Rolling 7-day average, updated daily |
| **Target** | No ingredient should reach zero before the next scheduled order |
| **Threshold — Green** | Projected stockout > 4 days |
| **Threshold — Amber** | Projected stockout = 2–3 days |
| **Threshold — Red** | Projected stockout ≤ 1 day |
| **Business Objective** | Enable proactive ordering decisions rather than reactive emergency purchasing |

---

# KPI-004: Top Selling Item — Daily

| Field | Detail |
|---|---|
| **Definition** | The single menu item with the highest units sold on a given day |
| **Formula** | MAX (Units Sold) across all menu items for the day |

:contentReference[oaicite:4]{index=4}

| **Data Source** | Excel sales log |
| **Frequency** | Daily |
| **Target** | Informational only — no pass/fail threshold |
| **Display Format** | Item name + units sold + revenue contribution |
| **Business Objective** | Help identify high-performing items to prioritise stock availability and preparation planning |

---

# KPI-005: Revenue vs Prior Week Variance

| Field | Detail |
|---|---|
| **Definition** | Percentage change in gross revenue compared to the equivalent day in the prior week |
| **Formula** | ((This Week Revenue − Last Week Revenue) ÷ Last Week Revenue) × 100 |

:contentReference[oaicite:5]{index=5}

| **Data Source** | Excel sales log — minimum 8 days of data required |
| **Frequency** | Daily |
| **Target** | ≥ 0% (flat or positive growth) |
| **Threshold — Green** | ≥ +5% |
| **Threshold — Amber** | −5% to +4.9% |
| **Threshold — Red** | < −5% |
| **Business Objective** | Provide a simple daily growth/decline signal without requiring manual comparison |

---

# KPI-006: Items Below Minimum Stock Threshold — Count

| Field | Detail |
|---|---|
| **Definition** | Number of ingredients currently at or below their defined minimum stock threshold |
| **Formula** | COUNT of ingredients where Current Stock ≤ Minimum Threshold |

:contentReference[oaicite:6]{index=6}

| **Data Source** | Excel inventory log — current stock vs threshold columns |
| **Frequency** | Real-time — updates on every data refresh |
| **Target** | 0 items below threshold at all times |
| **Threshold — Green** | 0 items |
| **Threshold — Amber** | 1–2 items |
| **Threshold — Red** | 3+ items |
| **Business Objective** | Provide an instant single-number alert requiring attention without scanning the entire inventory list |

---
