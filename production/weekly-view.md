# 🌾 Weekly Production View – Production Module

This view provides a **calendar-based matrix** of expected crop production per plot, week by week, aligned with forecasted demand and potential loss.  
Users can track **seeding**, **growing**, **ripening**, and **harvest** phases and interact with plots and crops to update tasks or review risks.

---

## 🧩 Component Breakdown

| Component Name            | Page Used              | Inherited? (from Shared) | React Ready?                            | Needs Customization?                  | Est. Time (hrs) | Priority | Status        |
| ------------------------- | ---------------------- | ------------------------ | --------------------------------------- | ------------------------------------- | --------------- | -------- | ------------- |
| **Sidebar Navigation**    | All Pages              | ✅ Yes                    | ✅ Yes (shadcn/ui)                       | Already implemented                   | —               | High     | ✅ Ready       |
| **Navbar – Top**          | All Pages              | ✅ Yes                    | ✅ Yes (shadcn/ui)                       | Already implemented                   | —               | High     | ✅ Ready       |
| **Filter – Crops**        | Weekly Production View | ✅ Yes                    | ✅ Yes (react-select / shadcn/ui Select) | Already implemented                   | —               | High     | ✅ Ready       |
| **Filter – Plots**        | Weekly Production View | ✅ Yes                    | ✅ Yes (react-select / shadcn/ui Select) | Already implemented                   | —               | High     | ✅ Ready       |
| **Filter – Tasks**        | Weekly Production View | ✅ Yes                    | ✅ Yes (react-select / shadcn/ui Select) | Already implemented                   | —               | High     | ✅ Ready       |
| **Week Selector (12–28)** | Weekly Production View | ✅ Yes                    | ⚠️ Partial (custom scroll needed)       | Horizontal scroll + sticky header     | __          | High     | ⬜ Not Started |
| **Timeline Grid View**    | Weekly Production View | ❌ No                     | ⚠️ Partial (shadcn/ui Table)            | Color-coded grid layout, row grouping | 4               | High     | ⬜ Not Started |
| **Production Icons Row**  | Weekly Production View | ❌ No                     | ⚠️ Partial (custom icons)               | Logic for icon rendering              | 2.5             | Medium   | ⬜ Not Started |
| **Legend (Color Keys)**   | Weekly Production View | ❌ No                     | ✅ Yes (custom card or tooltip list)     | Static component, color swatches      | 1               | Low      | ⬜ Not Started |
| **Indicators Toggle Bar** | Weekly Production View | ❌ No                     | ✅ Yes (shadcn/ui Toggle/Buttons)        | Requires context-based show/hide      | 1.5             | Medium   | ⬜ Not Started |
| **Tooltip – Icon Info**   | Weekly Production View | ✅ Yes                    | ✅ Yes (shadcn/ui Tooltip)               | Already implemented                   | —               | Medium   | ✅ Ready       |
| **Pagination Arrows**     | Weekly Production View | ✅ Yes                    | ✅ Yes (shadcn/ui Button or IconButton)  | Already implemented                   | —               | Medium   | ✅ Ready       |

---

## ⏱️ Total Estimated Time

| Component Type        | Description                                                | Time (hrs) |
|-----------------------|------------------------------------------------------------|------------|
| 🧩 **New Components** | Components that are **custom or partially reusable** and require implementation | **9 hrs** |
| ♻️ **Shared Components** | Components already implemented and reused here (from `general.md`) | **24.5 hrs** |
| ✅ **Total Combined Time** | Sum of new + shared component estimates for this view | **33.5 hrs** |

---

## 📘 Notes

- This view is **highly visual and grid-based**, and will likely require front-end optimization for scroll performance.
- Some components like dropdowns, tooltip, and date/week selectors are fully shared.
- Shared logic like filters and week navigation should be inherited directly from general UI setup.
- Chart rows like **Forecasted Demand** and **Potential Loss** are dynamically bound to external data.

---

## 🧭 To-Do

- [ ] Implement production grid layout
- [ ] Bind icons to crop stage logic
- [ ] Integrate shared filters and selectors
- [ ] Add responsive layout fallback
- [ ] Link to task modal on interaction
