# 👥 Client Forecast – Short-Term View (Sales)

This view displays **real-time insights on client behavior**, optimized for immediate action in the short-term (1–2 weeks).  
The indicators offer **precise metrics** such as performance delta, churn risk, and price sensitivity—helping sales managers respond to volatility quickly.

---

![Client Forecast – Short-Term](./images/sales-clients-short-term.png)

---

## 🧩 Component Breakdown

| Component Name             | Page Used              | Inherited? (from Shared) | React Ready?                            | Needs Customization?                          | Est. Time (hrs) | Priority | Status          | End Date |
|---------------------------|------------------------|--------------------------|-----------------------------------------|------------------------------------------------|------------------|----------|------------------|----------|
| **Sidebar Navigation**     | All Pages              | ✅ Yes                    | ✅ Yes (shadcn/ui)                       | Already implemented                           | —                | High     | ✅ Ready         |          |
| **Navbar – Top**           | All Pages              | ✅ Yes                    | ✅ Yes (shadcn/ui)                       | Already implemented                           | —                | High     | ✅ Ready         |          |
| **Filter – Clients**       | This Page              | ✅ Yes                    | ✅ Yes (shadcn/ui Select)                | Already implemented                           | —                | High     | ✅ Ready         |          |
| **Indicators Toggle Bar**  | This Page              | ✅ Yes                    | ✅ Yes (shadcn/ui Toggle)                | Show/hide grid rows                           | —                | High     | ✅ Ready         |          |
| **Real-Time Metrics Bar**  | This Page              | ❌ No                     | ❌ No                                    | Performance delta, churn risk, pricing alerts  | 3.5              | High     | ⬜ Not Started   |          |
| **Dynamic Table**          | This Page              | ⚠️ Partial (shared logic) | ⚠️ Partial                              | Shared structure + short-term data injection   | 3.5              | High     | ⬜ Not Started   |          |
| **Tooltip on Icons**       | This Page              | ✅ Yes                    | ✅ Yes (shadcn/ui Tooltip)               | Already implemented                           | —                | Medium   | ✅ Ready         |          |
| **Week Selector**          | This Page              | ✅ Yes                    | ⚠️ Partial                              | Horizontal scroll / sticky logic reused       | —                | High     | ✅ Ready         |          |
| **Pagination Arrows**      | This Page              | ✅ Yes                    | ✅ Yes                                   | Already implemented                           | —                | Medium   | ✅ Ready         |          |

---

## ⏱️ Total Estimated Time

| Component Type           | Description                                                  | Time (hrs) |
|--------------------------|--------------------------------------------------------------|------------|
| 🧩 **New Components**     | Real-time insights bar + table data customization            | **7 hrs** |
| ♻️ **Shared Components**  | Filters, navbar, sidebar, table, selectors                   | **~3 hrs** |
| ✅ **Total Combined Time**| Full page implementation estimate                           | **10 hrs** |

---

## 📘 Notes

- Client metrics are **immediate** (vs. projections in long-term), reflecting last-week comparisons and live churn risks.
- All indicators are **toggleable**, allowing users to show/hide sensitivity or retention rows.
- Grid content varies based on toggled indicators.
- All navigation and table logic are reused from long-term view with minimal customization.

---

## 🧭 To-Do

- [ ] Build short-term insight components (alerts, stats)
- [ ] Bind churn risk and sensitivity backend data
- [ ] Enable grid changes based on active indicators
- [ ] Optimize for desktop and tablet screen sizes
