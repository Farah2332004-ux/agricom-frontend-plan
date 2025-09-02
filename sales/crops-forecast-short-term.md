# 🌽 Crops Forecast – Short-Term View (Sales)

This view focuses on **immediate crop forecasting** by showing near-future sales signals like **price trends**, **demand**, **available stock**, and **order fulfillment**.  
The insights section provides **quantitative data** with actionable indicators for decision-making over the next 1–2 weeks.

---

![Crops Forecast – Short-Term](./images/sales-crops-short-term.png)

---

## 🧩 Component Breakdown

| Component Name             | Page Used              | Inherited? (from Shared) | React Ready?                            | Needs Customization?                          | Est. Time (hrs) | Priority | Status          | End Date |
|---------------------------|------------------------|--------------------------|-----------------------------------------|------------------------------------------------|------------------|----------|------------------|----------|
| **Sidebar Navigation**     | All Pages              | ✅ Yes                    | ✅ Yes (shadcn/ui)                       | Already implemented                           | —                | High     | ✅ Ready         |          |
| **Navbar – Top**           | All Pages              | ✅ Yes                    | ✅ Yes (shadcn/ui)                       | Already implemented                           | —                | High     | ✅ Ready         |          |
| **Filter – Crops**         | This Page              | ✅ Yes                    | ✅ Yes (shadcn/ui Select)                | Already implemented                           | —                | High     | ✅ Ready         |          |
| **Indicators Toggle Bar**  | This Page              | ✅ Yes                    | ✅ Yes (shadcn/ui Toggle)                | Show/hide rows dynamically                    | —                | High     | ✅ Ready         |          |
| **Insight Block – KPIs**   | This Page              | ❌ No                     | ❌ No                                    | Requires custom info block: availability, demand, price, fulfillment | 3.5              | High     | ⬜ Not Started   |          |
| **Dynamic Forecast Table** | This Page              | ⚠️ Partial (structure reused) | ⚠️ Partial (from general Table)     | Needs dynamic row toggle logic & indicator binding | 3.5              | High     | ⬜ Not Started   |          |
| **Tooltip on Icons**       | This Page              | ✅ Yes                    | ✅ Yes (shadcn/ui Tooltip)               | Already implemented                           | —                | Medium   | ✅ Ready         |          |
| **Week Selector**          | This Page              | ✅ Yes                    | ⚠️ Partial                              | Horizontal scroll / sticky logic reused       | —                | High     | ✅ Ready         |          |
| **Pagination Arrows**      | This Page              | ✅ Yes                    | ✅ Yes                                   | Already implemented                           | —                | Medium   | ✅ Ready         |          |

---

## ⏱️ Total Estimated Time

| Component Type          | Description                                                  | Time (hrs) |
|--------------------------|--------------------------------------------------------------|------------|
| 🧩 **New Components**     | Insight Block + table toggle logic                           | **7 hrs** |
| ♻️ **Shared Components**  | Navbar, sidebar, filters, table, tooltip, pagination         | **~3 hrs** |
| ✅ **Total Combined Time**| Estimated full page implementation time                     | **10 hrs** |

---

## 📘 Notes

- The **Insight KPI section** replaces the long-term forecast bars with detailed numbers and warning signals (e.g. 🔥 high price).
- The grid table remains the same component from the long-term view but dynamically populates different data.
- Toggle logic remains identical across views, ensuring reusability.
- Row headers (e.g. `Order Quantity`, `Revenue`, `Promo Linked`, `Channel Mix`) follow the same logic as other forecast tables.

---

## 🧭 To-Do

- [ ] Build and style insight info block
- [ ] Connect live short-term sales data
- [ ] Enable row toggling logic
- [ ] Ensure component reuse with long-term view
- [ ] Add warning logic (e.g. stock low, price high)
