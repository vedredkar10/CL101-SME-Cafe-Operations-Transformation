# As-Is & To-Be Process Desc Documentation
> BPMN Diagrams attached in frutilicious/Diagrams

**Project:** Frutilicious Café Analytics Solution  
**Business Analyst:** Ved Redkar | Visionize Consultancy LLP  
**Version:** 1.0  

---

# As-Is Process — Detailed Description

## Context

Prior to the engagement, Frutilicious Café operated with zero digital infrastructure for sales tracking, inventory management, or performance reporting. All operational knowledge lived in the owner's memory or in handwritten notebooks maintained by staff. The following describes the complete daily operational process as documented during elicitation sessions.

---

## Morning — Stock Assessment & Ordering (Owner)

The owner arrived at the café each morning and performed a mental stock check by walking through the storage area and visually estimating remaining quantities of each ingredient. There was no formal stock count process, no minimum threshold definition, and no historical consumption data to reference.

Ordering decisions were made entirely on instinct — the owner would call suppliers and place orders based on what he thought looked low, cross-referenced against a rough mental model of how busy the previous few days had been.

This process had two chronic failure modes:

1. Slow-moving items were consistently over-ordered because the owner could not accurately recall their depletion rate.
2. Fast-moving items — particularly those with high weekend demand — were under-ordered because the owner underestimated weekend uplift without supporting data.

Both failure modes contributed directly to wastage and stockout problems.

### Operational Characteristics

| Metric | Details |
|---|---|
| Estimated Time | 15–20 minutes daily |
| Accuracy | Low — entirely memory-dependent |
| Data Used | None |

---

## Service Hours — Sales Recording (Staff)

During service, staff recorded each sale in a physical notebook kept at the counter. The format was inconsistent — some staff wrote item names in full, others used abbreviations, and quantities were sometimes omitted if the café was busy.

There was no timestamp recorded against individual transactions. At the end of each service period, the notebook page was totalled manually by whichever staff member was closing, but this tally was frequently incomplete or inaccurate due to illegible handwriting or missed entries during peak periods.

The notebook was not reviewed by the owner in real time. If a popular item sold out mid-service, staff would either inform the owner verbally or simply stop serving it without any formal recording of the stockout event.

As a result, there was no data capture around stockout frequency or revenue impact.

### Operational Characteristics

| Metric | Details |
|---|---|
| Data Quality | Very low — inconsistent format, no timestamps, frequent gaps |
| Real-Time Visibility | None |
| Stockout Recording | None |

---

## End of Day — Tally & Review (Owner + Staff)

At the end of each day, the owner would review the notebook and attempt to calculate total sales. This involved manually adding quantities per item — a process that took 15–30 minutes and was prone to arithmetic errors.

Revenue was calculated approximately by multiplying estimated quantities by recalled prices, without a formal price list for reference.

There was no structured end-of-day review process. The owner could not reliably answer operational questions such as:

- What was today's gross revenue?
- Which item sold the most today?
- How does today compare to last week?
- What is the current stock of ingredient X?

All of these questions required either manual calculation or guesswork.

Weekly and monthly trend analysis was not performed at all. The owner had no visibility into seasonal trends, longer-term sales patterns, or menu performance over time.

### Operational Characteristics

| Metric | Details |
|---|---|
| Time to Generate Daily Summary | 15–30 minutes |
| Accuracy | Low |
| Trend Analysis | None |

---

## Ordering Cycle — Weekly (Owner)

Once or twice a week, the owner placed supplier orders based on the rough mental stock checks performed each morning, combined with intuition about expected demand.

There was:

- No consumption rate data
- No depletion projection
- No minimum stock threshold framework

The result was consistently suboptimal ordering:

- Some items were over-ordered, generating wastage when products expired
- Other items were under-ordered, generating stockouts and lost revenue

The owner estimated pre-engagement wastage at approximately **25% of total stock**, representing a major financial loss for a small independent café.

### Operational Characteristics

| Metric | Details |
|---|---|
| Decision Basis | Memory + intuition |
| Estimated Wastage Rate | ~25% |
| Stockout Frequency | Regular, unquantified |

---

# Summary of As-Is Pain Points

- No digital data capture — all sales recorded in inconsistent handwritten notebooks
- No real-time visibility — owner blind to performance until manual end-of-day tally
- No revenue tracking — gross revenue calculated manually and inaccurately
- No inventory system — stock levels estimated visually from memory
- No wastage recording — wastage unquantified and untracked
- No trend analysis — no week-on-week, day-of-week, or item-level performance data
- No alerts — stockouts discovered only when items ran out during service
- Decision latency — ordering decisions made on stale, inaccurate information

---

# To-Be Process — Detailed Description

## Context

Following requirements elicitation, the To-Be process was designed around two core principles:

1. **Simplicity of data entry for staff**
2. **Richness of insight for the owner**

The solution had to:

- Require zero technical knowledge
- Be accessible on mobile devices
- Deliver actionable information in under 60 seconds each morning

---

## Morning — Dashboard Review & Ordering Decision (Owner)

The owner opens the Power BI dashboard on a phone or desktop at the start of each day.

The home screen immediately displays six KPI cards:

- Today's Gross Revenue (vs yesterday)
- Units Sold Yesterday
- Top Selling Item
- Wastage % This Week
- Stock Alert Count
- Revenue vs Prior Week Variance

This enables the owner to assess business health in under 60 seconds without manual calculations.

If the **Stock Alert Count** KPI shows flagged items, the owner navigates to the inventory panel, which displays:

- Current estimated stock levels
- Amber/red threshold alerts
- Projected days-until-stockout figures

Supplier orders are now placed using actual consumption data rather than intuition.

### Operational Characteristics

| Metric | Details |
|---|---|
| Estimated Time | 3–5 minutes daily |
| Accuracy | High — based on actual logged data |
| Data Used | Live Excel data via SharePoint connection |

---

## Service Hours — Digital Sales Logging (Staff)

Staff log each sale directly into a structured Excel workbook hosted on SharePoint.

The workbook includes three required fields:

| Field | Description |
|---|---|
| Menu Item | Selected from validated drop-down list |
| Quantity Sold | Numeric quantity entry |
| Time of Sale | Timestamp for transaction |

The drop-down structure prevents free-text inconsistencies and ensures standardised data capture.

Staff can access the workbook using:

- Shared tablet
- Personal mobile device

Wastage is logged separately at the end of each service period by recording:

- Item wasted
- Quantity wasted

Because the workbook is hosted on SharePoint and connected live to Power BI, all updates appear automatically in the dashboard without manual refreshes or exports.

### Operational Characteristics

| Metric | Details |
|---|---|
| Data Quality | High — validated, structured, timestamped |
| Real-Time Visibility | Immediate |
| Stockout Recording | Logged in designated column |

---

## During Service — Live Monitoring (Owner, Optional)

The owner can monitor performance live from any internet-connected device during service hours.

If a particular item begins selling unusually quickly, the owner can:

- Prepare additional stock proactively
- Alert staff before stockout occurs

The hourly sales breakdown page compares current-hour sales against historical averages and highlights unusual activity patterns.

### Operational Characteristics

| Metric | Details |
|---|---|
| Availability | Any time, any device with internet access |
| Data Lag | Near real-time — updates within minutes |

---

## End of Day — Automated Summary (System)

In the To-Be state, there is no manual end-of-day tally process.

All calculations are automated through Power BI DAX measures, including:

- Gross revenue
- Units sold
- Wastage percentage
- Stock depletion

The dashboard automatically reflects complete daily performance without manual intervention.

The owner can instantly review:

- Daily performance summary
- Weekly trends
- Monthly item rankings
- Day-of-week comparisons

### Operational Characteristics

| Metric | Details |
|---|---|
| Time to Generate Daily Summary | 0 minutes — fully automated |
| Accuracy | High — based on logged transactional data |
| Trend Analysis | Automated — weekly, monthly, hourly |

---

## Ordering Cycle — Data-Driven (Owner)

Supplier ordering is now based on live inventory data rather than memory.

The owner reviews:

- Projected days-until-stockout
- Weekly sales trends
- Weekend demand uplift
- Minimum stock threshold alerts

Orders are calibrated using actual consumption rates and projected demand.

This creates a proactive inventory management process instead of reactive emergency ordering.

### Operational Characteristics

| Metric | Details |
|---|---|
| Decision Basis | Actual consumption data + depletion projections |
| Wastage Rate | Reduced to <10% within first month |
| Stockout Frequency | Significantly reduced |

---

# Summary of To-Be Improvements

| As-Is | To-Be | Improvement |
|---|---|---|
| Handwritten notebook | Structured Excel with validated drop-downs | Consistent, analysable data |
| No revenue tracking | Automated gross revenue KPI | Accurate daily revenue in seconds |
| Memory-based stock check | Live inventory panel with alerts | Proactive, data-driven ordering |
| No wastage recording | Daily wastage log + dashboard KPI | Quantified and trackable wastage |
| No trend analysis | Weekly, monthly, hourly dashboards | Full performance visibility |
| 15–30 minute daily tally | Fully automated summaries | Significant time savings |
| ~25% wastage rate | <10% wastage rate | ~20% reduction achieved |
| Stockouts during service | Proactive threshold alerts | Stockouts significantly reduced |

---
