# 🌽 Crops Forecast – Long-Term View (Sales)

This page displays the long-term forecast of crop performance week by week, helping the team anticipate **demand**, **price fluctuation**, and **profitability windows**.  
Users can toggle visibility of multiple indicators, dynamically altering the table view.

---

![Crops Forecast – Long-Term](./images/sales-crops-long-term.png)

---

## 🧩 Component Breakdown

| Component Name             | Page Used              | Inherited? (from Shared) | React Ready?                            | Needs Customization?                          | Est. Time (hrs) | Priority | Status          | End Date |
|---------------------------|------------------------|--------------------------|-----------------------------------------|------------------------------------------------|------------------|----------|------------------|----------|
| **Sidebar Navigation**     | All Pages              | ✅ Yes                    | ✅ Yes (shadcn/ui)                       | Already implemented                           | —                | High     | ✅ Ready         |          |
| **Navbar – Top**           | All Pages              | ✅ Yes                    | ✅ Yes (shadcn/ui)                       | Already implemented                           | —                | High     | ✅ Ready         |          |
| **Filter – Crops**         | This Page              | ✅ Yes                    | ✅ Yes (shadcn/ui Select)                | Already implemented                           | —                | High     | ✅ Ready         |          |
| **Indicators Toggle Bar**  | This Page              | ✅ Yes                    | ✅ Yes (shadcn/ui Toggle)                | Show/hide rows dynamically                    | —                | High     | ✅ Ready         |          |
| **Forecast Demand Bar**    | This Page              | ❌ No                     | ❌ No                                    | Requires custom forecast logic & coloring     | 3                | High     | ⬜ Not Started   |          |
| **Forecast Price Bar**     | This Page              | ❌ No                     | ❌ No                                    | Price zones + peak price alert icon           | 3                | High     | ⬜ Not Started   |          |
| **Dynamic Forecast Table** | This Page              | ⚠️ Partial (structure reused) | ⚠️ Partial (from general Table)     | Needs dynamic row toggle logic & indicator binding | 3.5              | High     | ⬜ Not Started   |          |
| **Tooltip on Icons**       | This Page              | ✅ Yes                    | ✅ Yes (shadcn/ui Tooltip)               | Already implemented                           | —                | Medium   | ✅ Ready         |          |
| **Week Selector**          | This Page              | ✅ Yes                    | ⚠️ Partial                              | Horizontal scroll / sticky logic reused       | —                | High     | ✅ Ready         |          |
| **Pagination Arrows**      | This Page              | ✅ Yes                    | ✅ Yes                                   | Already implemented                           | —                | Medium   | ✅ Ready         |          |

---

## ⏱️ Total Estimated Time

| Component Type          | Description                                                  | Time (hrs) |
|--------------------------|--------------------------------------------------------------|------------|
| 🧩 **New Components**     | Forecast bars, toggle logic, dynamic table                   | **9.5 hrs** |
| ♻️ **Shared Components**  | Navbar, sidebar, filters, tooltips, week selector, arrows    | **~4.5 hrs** |
| ✅ **Total Combined Time**| Estimated full page implementation time                     | **14 hrs** |

---

## 📘 Notes

- Dynamic row toggling logic is critical here — each selected indicator shows new data rows (e.g., `Order Quantity`, `Promo Linked`, `Revenue`).
- Forecast bars use **custom visual scales** and **alert icons** to guide stock and pricing decisions.
- Page structure builds on existing production-style tables but overlays **sales logic**.
- Reused components (filters, navbar, sidebar) should already be globally available from the shared layer.

---

## 🧭 To-Do

- [ ] Implement Forecast Demand & Price bars
- [ ] Hook toggle bar to dynamic row logic
- [ ] Bind rows per crop + indicator toggle
- [ ] Ensure chart responsiveness
- [ ] Link to crop-level pages as needed
