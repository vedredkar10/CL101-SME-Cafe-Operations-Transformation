# Gap Analysis Documentation

**Project:** Frutilicious Café Analytics Solution  
**Business Analyst:** Ved Redkar | Visionize Consultancy LLP  
**Version:** 1.0  

---

## Methodology

Gap analysis was conducted through structured stakeholder interviews with the café owner across two elicitation sessions. The *As-Is* state was documented by observing current operations and asking the owner to walk through a typical working day. Pain points were captured verbatim and then categorised. The *To-Be* state was defined collaboratively with the owner based on his stated needs and the constraints of a low-budget, non-technical solution.

---

# Gap Analysis Table

| Gap ID | Business Area | As-Is (Current State) | Pain Point | To-Be (Desired State) | Solution Delivered |
|---|---|---|---|---|---|
| **GAP-001** | Sales Tracking | Staff record all sales manually in a physical notebook at the end of each transaction | Data is illegible, incomplete, and impossible to aggregate or analyse | Staff log sales digitally in a structured Excel sheet with predefined columns for item, quantity, and timestamp | Structured Excel sales log template designed with validated drop-down item lists to prevent data entry errors |
| **GAP-002** | Revenue Visibility | Owner calculates approximate daily revenue mentally or not at all | No accurate daily revenue figure available — owner has no idea if a day was profitable | Gross revenue calculated automatically and displayed on Power BI dashboard as a live KPI | Power BI measure created using DAX formula to auto-calculate revenue from quantity × unit price |
| **GAP-003** | Inventory Management | Owner estimates stock levels from memory each morning before ordering | Frequent over-ordering of slow items and under-ordering of fast items leading to wastage and stockouts simultaneously | Live stock level estimates visible on dashboard with red/amber/green threshold indicators | Inventory tracking tab added to Excel, connected to dashboard inventory panel |
| **GAP-004** | Wastage Tracking | No wastage is formally recorded — owner estimates wastage as "a lot" with no data | Impossible to identify which items are wasted most or quantify the financial impact | Staff log wastage quantities daily, dashboard displays wastage % per item and total wastage cost | Wastage column added to Excel log, wastage KPI card added to dashboard home screen |
| **GAP-005** | Sales Pattern Awareness | Owner has no visibility into which items sell best on which days or at which times | Staffing and stock decisions are made uniformly regardless of day-of-week variation | Dashboard displays weekday vs weekend sales split and peak hour analysis | Weekly and hourly breakdown pages added to Power BI dashboard |
| **GAP-006** | Data Freshness | Any analysis the owner wanted to do required manually totalling the notebook — done at most weekly | Decisions were always based on stale, incomplete data | Dashboard connected live to Excel via SharePoint — refreshes automatically when new data is entered | SharePoint-hosted Excel workbook connected to Power BI via live data connection |
| **GAP-007** | Decision-Making Speed | Owner spent 15–20 minutes each morning trying to recall yesterday's performance before making ordering decisions | Slow, unreliable morning decision process leading to suboptimal orders | Owner opens dashboard on phone or desktop — full picture visible in under 60 seconds | Mobile-responsive Power BI dashboard published to Power BI Service |
| **GAP-008** | Menu Performance | No mechanism to identify underperforming menu items — items stayed on menu indefinitely regardless of sales | Menu carried items that generated minimal revenue and consumed storage and prep time | Monthly top/bottom item ranking visible on dashboard to inform menu review decisions | Monthly performance page with ranked item table added to dashboard |

---

# Summary of Gaps by Category

| Category | Number of Gaps | Severity |
|---|---|---|
| Data Capture & Quality | 2 (GAP-001, GAP-004) | High |
| Visibility & Reporting | 3 (GAP-002, GAP-005, GAP-008) | High |
| Inventory & Wastage | 2 (GAP-003, GAP-006) | Critical |
| Decision-Making Speed | 1 (GAP-007) | Medium |

---
