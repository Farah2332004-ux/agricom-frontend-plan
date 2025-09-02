# 👥 Client Forecast – Long-Term View (Sales)

This view shows **client-related sales projections** over several upcoming weeks. It focuses on **behavioral trends**, such as **client performance** and **price sensitivity**, enabling strategic decisions around retention, targeting, and inventory prioritization.

---

![Client Forecast – Long-Term](./images/sales-clients-long-term.png)

---

## 🧩 Component Breakdown

| Component Name             | Page Used              | Inherited? (from Shared) | React Ready?                            | Needs Customization?                          | Est. Time (hrs) | Priority | Status          | End Date |
|---------------------------|------------------------|--------------------------|-----------------------------------------|------------------------------------------------|------------------|----------|------------------|----------|
| **Sidebar Navigation**     | All Pages              | ✅ Yes                    | ✅ Yes (shadcn/ui)                       | Already implemented                           | —                | High     | ✅ Ready         |          |
| **Navbar – Top**           | All Pages              | ✅ Yes                    | ✅ Yes (shadcn/ui)                       | Already implemented                           | —                | High     | ✅ Ready         |          |
| **Filter – Clients**       | This Page              | ✅ Yes                    | ✅ Yes (shadcn/ui Select)                | Already implemented                           | —                | High     | ✅ Ready         |          |
| **Indicators Toggle Bar**  | This Page              | ✅ Yes                    | ✅ Yes (shadcn/ui Toggle)                | Show/hide rows dynamically                    | —                | High     | ✅ Ready         |          |
| **Forecast Insight Bars**  | This Page              | ❌ No                     | ❌ No                                    | Client performance + sensitivity forecast bars | 3.5              | High     | ⬜ Not Started   |          |
| **Dynamic Table**          | This Page              | ⚠️ Partial (shared logic) | ⚠️ Partial                              | Reused structure, new data binding             | 3.5              | High     | ⬜ Not Started   |          |
| **Tooltip on Icons**       | This Page              | ✅ Yes                    | ✅ Yes (shadcn/ui Tooltip)               | Already implemented                           | —                | Medium   | ✅ Ready         |          |
| **Week Selector**          | This Page              | ✅ Yes                    | ⚠️ Partial                              | Horizontal scroll / sticky logic reused       | —                | High     | ✅ Ready         |          |
| **Pagination Arrows**      | This Page              | ✅ Yes                    | ✅ Yes                                   | Already implemented                           | —                | Medium   | ✅ Ready         |          |

---

## ⏱️ Total Estimated Time

| Component Type          | Description                                                  | Time (hrs) |
|--------------------------|--------------------------------------------------------------|------------|
| 🧩 **New Components**     | Insight forecast bars + table binding                        | **7 hrs** |
| ♻️ **Shared Components**  | Filters, navbar, sidebar, table, selectors                   | **~3 hrs** |
| ✅ **Total Combined Time**| Full page implementation estimate                           | **10 hrs** |

---

## 📘 Notes

- **Client performance** highlights active/inactive clients across the planning horizon.
- **Price sensitivity** indicates groups responsive to discounts or price changes.
- Toggle bar logic mirrors crop views: turning indicators on/off controls grid rows.
- Table content reflects long-term estimations, not real-time orders.
- All interaction patterns are inherited from existing sales components.

---

## 🧭 To-Do

- [ ] Design and implement insight forecast bars
- [ ] Connect to client metrics from backend
- [ ] Enable row toggling behavior per indicator
- [ ] Reuse table logic from crop forecast view
- [ ] Implement alert thresholds for performance drop or high sensitivity
