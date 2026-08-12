# 💳 Treasury Vista — Finance Analytics Dashboard

An interactive **Power BI** dashboard built for a financial organization to monitor and analyze transaction performance, customer behavior, fees, taxes, and regional trends — enabling faster, data-driven financial decision-making.

## 📌 Business Objective

Management needed a centralized analytical solution to track:

- Overall transaction growth and financial performance
- Monthly trends in transaction amounts
- Successful vs. failed transactions
- Customer segment contribution
- State-wise financial performance
- Transaction type profitability
- Gender-based customer analysis
- Year-over-Year (YoY) performance changes

The dashboard gives stakeholders a single place to monitor KPIs in real time, spot high-performing customer segments and states, track fees and taxes, and understand customer demographics.

---

## 🧭 Dashboard Pages

### 1. Overview
- KPI cards: **Total Amount, Total Transactions, Average Transaction Value, Total Fees, Total Tax** — each with YoY comparison
- Additional KPI cards for **Success %** and **Male %**
- Total Amount by Month — line chart, for spotting seasonal trends
- Total Amount by Transaction Status — donut chart (Success / Failed / Pending)
- Total Amount by Customer Segment — horizontal bar chart (Retail, Premium, SME, Corporate, Wealth)
- Total Amount by Gender — donut chart
- Filters: Year, Occupation, Category, Dynamic Parameter

### 2. Region
- Total Amount by State — horizontal bar chart, for comparing regional performance
- Transaction Type Analysis table — Amount, Fees, Tax and Transaction Count broken down by type (Bill Payment, Card Payment, Deposit, Fee Charge, Interest Credit, Investment, Loan EMI, Refund, Transfer, Withdrawal)
- Filters: Year, Occupation, Category, Dynamic Parameter

### 3. Detailed View
- Full transaction-level data grid: Transaction ID, Date, Customer Name, Transaction Type, Status, Gender, Occupation, Merchant Category, State, Amount
- Filters: Year, City, Category, Dynamic Parameter
- Action button to clear all filters

---

## 🛠️ Tools & Skills Used

- **Power BI Desktop** — end-to-end report building
- **DAX** — KPI measures, YoY growth calculations, % calculations (Success %, Male %)
- **Power Query** — data cleaning and transformation across the customers and transactions tables
- **Data Modeling** — relationships between `finance_transactions`, `customers`, and a `Calendar` table, plus a Dynamic Parameter for flexible measure switching
- **Data Visualization** — line charts, donut charts, bar charts, KPI cards, and a transaction-level data table
- **Interactivity** — slicers, cross-filtering, and navigation buttons across pages

---

## 🗃️ Data Model

| Table | Purpose |
|---|---|
| `finance_transactions` | Core transaction records — type, status, amount, fees, tax, date, merchant category |
| `customers` | Customer attributes — segment, gender, occupation, state, city |
| `Calendar Table` | Date table powering time intelligence (Month, Year, YoY comparisons) |
| `Dynamic Parameter` | Lets users switch between measures dynamically on charts |

 ## 📁 Repository Structure
treasury-vista-dashboard/
├── Treasury_Vista.pbix
├── screenshots/
│   ├── overview.png
│   ├── region.png
│   └── detailed_view.png
└── README.md


