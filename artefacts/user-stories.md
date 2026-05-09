# User Stories & Acceptance Criteria

## Project Information

| Field | Details |
|---|---|
| **Project** | Frutilicious Café Analytics Solution |
| **Business Analyst** | Ved Redkar \| Visionize Consultancy LLP |
| **Version** | 1.0 |

---

# Epic 1: Sales Visibility

## US-001: Daily Sales by Item

### User Story
As a café owner, I want to see how many units of each menu item were sold today, so that I can understand which items are performing well and which are not.

### AC
- Given the staff have logged all sales for the day into the Excel sheet  
- When the owner opens the Power BI dashboard  
- Then he should see a bar chart showing units sold per menu item for the current day  
- And items should be sortable from highest to lowest sales  
- And the data should reflect sales up to the last Excel entry without manual refresh  

| Priority | Story Points |
|---|---|
| Must Have | 3 |

---

## US-002: Weekly Sales Trends

### User Story
As a café owner, I want to see sales trends over the past 7 days for each menu item, so that I can identify patterns and adjust my ordering accordingly.

### AC
- Given at least 7 days of sales data has been logged  
- When the owner navigates to the weekly view on the dashboard  
- Then he should see a line chart showing daily units sold per item over the past 7 days  
- And the chart should highlight the highest and lowest performing days visually  
- And the owner should be able to filter by individual menu item  

| Priority | Story Points |
|---|---|
| Must Have | 3 |

---

## US-003: Gross Revenue — Daily

### User Story
As a café owner, I want to see my total gross revenue for today, so that I know how much money the café has taken in before any deductions.

### AC
- Given each menu item has a unit price defined in the Excel sheet  
- When sales quantities are logged by staff  
- Then the dashboard should automatically calculate gross revenue as units sold × unit price per item  
- And display a total gross revenue figure prominently on the dashboard home screen  
- And show a breakdown of revenue contribution per item  

| Priority | Story Points |
|---|---|
| Must Have | 2 |

---

## US-004: Gross Revenue vs Prior Week Comparison

### User Story
As a café owner, I want to compare today's gross revenue against the same day last week, so that I can quickly assess whether the business is growing or declining.

### AC
- Given at least 8 days of revenue data exists  
- When the owner views the revenue summary on the dashboard  
- Then he should see today's gross revenue alongside last week's equivalent day  
- And a percentage change indicator (up/down arrow) should display the variance  
- And positive variance should display in green, negative in red  

| Priority | Story Points |
|---|---|
| Must Have | 3 |

---

## US-005: Peak Hours Identification

### User Story
As a café owner, I want to know which hours of the day generate the most sales, so that I can schedule staff appropriately and ensure popular items are adequately stocked during rush periods.

### AC
- Given staff log sales with a timestamp for each transaction  
- When the owner views the hourly sales breakdown  
- Then the dashboard should display a heatmap or bar chart showing sales volume by hour of day  
- And the top 3 peak hours should be highlighted  
- And the owner should be able to filter by day of week to see if peak hours vary  

| Priority | Story Points |
|---|---|
| Should Have | 5 |

---

## US-006: Weekend vs Weekday Sales Split

### User Story
As a café owner, I want to see how my sales split between weekdays and weekends, so that I can plan staffing and stock ordering differently for each period.

### AC
- Given sales data has been logged with dates for at least 2 weeks  
- When the owner views the weekly breakdown panel  
- Then the dashboard should display average daily sales for weekdays vs weekends separately  
- And show which menu items perform significantly better on weekends vs weekdays  
- And this view should update automatically as new data is added  

| Priority | Story Points |
|---|---|
| Should Have | 3 |

---

# Epic 2: Inventory Management

## US-007: Current Stock Level Visibility

### User Story
As a café owner, I want to see current stock levels for all ingredients without having to physically count them, so that I can make faster and more accurate ordering decisions.

### AC
- Given opening stock levels and daily usage rates are logged in the Excel sheet  
- When the owner opens the inventory panel on the dashboard  
- Then he should see current estimated stock levels per ingredient  
- And items below a defined threshold should be highlighted in amber or red  
- And the view should reflect the most recently entered data  

| Priority | Story Points |
|---|---|
| Must Have | 5 |

---

## US-008: Low Stock Alerts

### User Story
As a café owner, I want to be alerted when any ingredient drops below a minimum threshold, so that I can reorder before running out and avoid stockouts during service.

### AC
- Given minimum stock thresholds have been defined for each ingredient  
- When estimated stock falls at or below the threshold  
- Then the dashboard should display a visual alert — highlighted row in red with an alert icon  
- And the alert should list the ingredient name, current estimated level, and minimum threshold  
- And the alert should persist until stock is replenished and updated in the Excel sheet  

| Priority | Story Points |
|---|---|
| Must Have | 3 |

---

## US-009: Inventory Depletion Rate

### User Story
As a café owner, I want to see how quickly each ingredient is being consumed on average, so that I can predict when I will run out and order proactively.

### AC
- Given at least 2 weeks of sales and usage data has been logged  
- When the owner views the inventory analytics panel  
- Then the dashboard should display average daily consumption rate per ingredient  
- And show a projected days-until-stockout figure based on current stock and depletion rate  
- And flag any ingredient projected to run out within 3 days  

| Priority | Story Points |
|---|---|
| Should Have | 5 |

---

## US-010: Wastage Tracking

### User Story
As a café owner, I want to log and track daily wastage per ingredient, so that I can identify which items are being over-ordered and reduce unnecessary costs.

### AC
- Given staff log wastage quantities daily in the designated Excel column  
- When the owner views the wastage panel  
- Then the dashboard should display total wastage per ingredient over the selected period  
- And calculate wastage as a percentage of total stock used  
- And highlight the top 3 most wasted items to focus reduction efforts  

| Priority | Story Points |
|---|---|
| Must Have | 3 |

---

# Epic 3: KPI Reporting

## US-011: Dashboard Home KPI Summary

### User Story
As a café owner, I want to see all my key performance indicators on a single screen when I open the dashboard, so that I can get an instant overview of business health without navigating multiple pages.

### AC
- Given the dashboard has been opened and data is current  
- When the owner lands on the home screen  
- Then he should see the following KPIs displayed as cards:  
  - Today's Gross Revenue  
  - Units Sold Today  
  - Top Selling Item Today  
  - Wastage % This Week  
  - Stock Alert Count  
  - Revenue vs Last Week %  
- And each KPI card should have a clear label, value, and trend indicator  
- And the layout should be readable on both desktop and mobile browser  

| Priority | Story Points |
|---|---|
| Must Have | 5 |

---

## US-012: Top and Bottom Performing Items

### User Story
As a café owner, I want to see a ranked list of my best and worst performing menu items over the past month, so that I can make informed decisions about menu changes.

### AC
- Given at least 30 days of sales data exists  
- When the owner views the monthly performance panel  
- Then the dashboard should display the top 5 and bottom 5 menu items ranked by units sold  
- And show revenue contribution alongside units sold for each item  
- And allow the owner to toggle between current month and previous month for comparison  

| Priority | Story Points |
|---|---|
| Could Have | 3 |
