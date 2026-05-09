# frutilicious-cafe-ba

# Frutilicious Café — Business Analysis Documentation & Process

**Author:** Ved Redkar | Co-Founder & Analytics Associate, Visionize Consultancy LLP
**Client:** Frutilicious Café, Panjim-Goa, India
**Engagement Type:** End-to-end Business Analysis Lifecycle & Analytics Solution Delivery
**Timeline:** 2022-23
**Status:** Delivered

---

## Project Outline

Frutilicious Café was a growing independent café in Goa operating entirely on
institutional memory and handwritten notebooks. The owner had no visibility
into daily sales, revenue, inventory levels, or wastage — all ordering and
operational decisions were made on intuition. This engagement involved
conducting full requirements elicitation, defining KPIs, designing As-Is and
To-Be processes using BPMN, and delivering an automated Power BI dashboard
solution connected live via SharePoint.

**Outcome:** 20% reduction in inventory wastage within the first month of
deployment.

---

## Problem Statement

The café owner was experiencing two simultaneous operational problems:

1. **Inventory wastage** — slow-moving items were consistently over-ordered
   because there was no consumption data to reference, resulting in stock
   expiring before it could be sold.

2. **Stockouts** — fast-moving items, particularly those with high weekend
   demand, were under-ordered because the owner had no visibility into
   day-of-week sales patterns.

Both problems stemmed from the same root cause: **zero data infrastructure**.
Every decision — ordering, staffing, menu management — was made without a
single piece of recorded, analysable data. Pre-engagement wastage was
estimated at approximately 25% of total stock.

---

## My Role

- **Business Analyst** — sole BA on the engagement
- **Solution Designer** — defined the data architecture and dashboard
  structure
- **Stakeholder Manager** — conducted all elicitation sessions with the
  café owner
- **Requirements Owner** — wrote all user stories, acceptance criteria,
  and KPI definitions
- **Bridge between business and technical** — translated requirements to
  my co-founder (technical implementer) who built the Excel + SharePoint
  + Power BI solution

---

## BA Techniques Deployed

| Technique | Application |
|---|---|
| Requirements Elicitation | Structured stakeholder interviews with café owner across 2 sessions |
| User Story Writing | 12 user stories written across 3 epics with full acceptance criteria |
| Acceptance Criteria (Given/When/Then) | Defined for all Must Have and Should Have stories |
| KPI Definition | 6 KPIs defined, measured, and implemented on dashboard |
| As-Is Process Mapping | Full current-state process documented across owner and staff swimlanes |
| To-Be Process Design | Future-state process designed with system swimlane added |
| BPMN Process Modelling | As-Is and To-Be BPMN diagrams produced using Draw.io |
| Gap Analysis | 8 gaps identified across 4 categories with severity ratings |
| MoSCoW Prioritisation | All user stories prioritised using MoSCoW framework |
| UAT (informal) | Dashboard reviewed with owner against original requirements, iterated |

---

## Tools Used

| Tool | Purpose |
|---|---|
| Draw.io | BPMN As-Is and To-Be process diagrams |
| Microsoft Excel | Data capture layer — sales log, inventory log, wastage log |
| SharePoint | Live data hosting — Excel workbook connected to Power BI |
| Power BI | Dashboard development, KPI visualisation, DAX measures |
| Power BI Service | Dashboard publishing for mobile access |

---

## Epics & User Stories Overview

### Epic 1: Sales Visibility
| Story ID | Title | Priority |
|---|---|---|
| US-001 | Daily Sales by Item | Must Have |
| US-002 | Weekly Sales Trends | Must Have |
| US-003 | Gross Revenue — Daily | Must Have |
| US-004 | Gross Revenue vs Prior Week Comparison | Must Have |
| US-005 | Peak Hours Identification | Should Have |
| US-006 | Weekend vs Weekday Sales Split | Should Have |

### Epic 2: Inventory Management
| Story ID | Title | Priority |
|---|---|---|
| US-007 | Current Stock Level Visibility | Must Have |
| US-008 | Low Stock Alerts | Must Have |
| US-009 | Inventory Depletion Rate | Should Have |
| US-010 | Wastage Tracking | Must Have |

### Epic 3: KPI Reporting
| Story ID | Title | Priority |
|---|---|---|
| US-011 | Dashboard Home KPI Summary | Must Have |
| US-012 | Top and Bottom Performing Items | Could Have |

---

## KPI Summary

| KPI ID | KPI Name | Target | Frequency |
|---|---|---|---|
| KPI-001 | Daily Gross Revenue | ≥ daily target | Daily |
| KPI-002 | Inventory Wastage % | < 10% per week | Weekly |
| KPI-003 | Stock Depletion Rate | No stockout within order cycle | Rolling 7-day |
| KPI-004 | Top Selling Item | Informational | Daily |
| KPI-005 | Revenue vs Prior Week Variance | ≥ 0% | Daily |
| KPI-006 | Items Below Minimum Stock Threshold | 0 items | Real-time |

---

## Gap Analysis Summary

| Gap ID | Area | Severity |
|---|---|---|
| GAP-001 | Sales data capture | High |
| GAP-002 | Revenue visibility | High |
| GAP-003 | Inventory management | Critical |
| GAP-004 | Wastage tracking | Critical |
| GAP-005 | Sales pattern awareness | High |
| GAP-006 | Data freshness | High |
| GAP-007 | Decision-making speed | Medium |
| GAP-008 | Menu performance visibility | Medium |

Full gap analysis with As-Is, pain point, To-Be, and solution delivered
for each gap → [`/artefacts/gap-analysis.md`](./artefacts/gap-analysis.md)

---

## Process Diagrams (BPMN)

### As-Is Process
The pre-engagement process involved entirely manual, memory-based operations
across owner and staff with no digital infrastructure, no real-time
visibility, and no data capture beyond a handwritten notebook.

![As-Is BPMN Diagram](./artefacts/diagrams/asis-bpmn.png)

### To-Be Process
The post-engagement process introduced a digital sales logging system,
live SharePoint-connected Excel workbook, and automated Power BI dashboard
accessible in real time on mobile or desktop.

![To-Be BPMN Diagram](./artefacts/diagrams/tobe-bpmn.png)

Full written process descriptions (As-Is and To-Be) →
[`/artefacts/asis-tobe-process.md`](./artefacts/asis-tobe-process.md)

---

## 📐 Solution Architecture
