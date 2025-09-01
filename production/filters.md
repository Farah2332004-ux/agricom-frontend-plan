# 🔽 Filters – Production Module

Filters are used to refine the view based on selected **Crops**, **Plots**, and **Tasks**. They are persistent across production pages and adapt based on the page context (e.g., timeline vs simulator).

---

## 🧩 Component Breakdown

| Component Name           | Page Used            | Inherited? (from Shared) | React Ready?                            | Needs Customization?               | Est. Time (hrs) | Priority | Status        | End Date |
| ------------------------ | -------------------- | ------------------------ | --------------------------------------- | ---------------------------------- | --------------- | -------- | ------------- | -------- |
| **Filter – Crops**       | All Production Pages | ✅ Yes                    | ✅ Yes (react-select / shadcn/ui Select) | Shared filter with dropdown        | —               | High     | ✅ Ready       |          |
| **Filter – Plots**       | All Production Pages | ✅ Yes                    | ✅ Yes (react-select / shadcn/ui Select) | Shared filter with dropdown        | —               | High     | ✅ Ready       |          |
| **Filter – Tasks**       | All Production Pages | ✅ Yes                    | ✅ Yes (react-select / shadcn/ui Select) | Shared filter with dropdown        | —               | High     | ✅ Ready       |          |
| **Filter Panel Wrapper** | All Production Pages | ⚠️ Partial               | ⚠️ Partial                              | Grouped filters, responsive layout | 2.5             | High     | ⬜ Not Started |          |
| **Clear Filters Button** | All Production Pages | ❌ No                     | ✅ Yes (shadcn/ui Button)                | Resets all filters                 | 0.5             | Medium   | ⬜ Not Started |          |

---

## ⏱️ Total Estimated Time

| Component Type            | Description                                         | Time (hrs)  |
| ------------------------- | --------------------------------------------------- | ----------- |
| 🧩 **New Components**     | Custom or adapted wrappers like filter group layout | **3 hrs**   |
| ♻️ **Shared Components**  | Dropdowns reused from shared component plan         | **2.5 hrs** |
| ✅ **Total Combined Time** | Sum of new + shared component estimates for filters | **6.5 hrs** |

---

## 📘 Notes

* The dropdowns are fully shared and already built.
* Filter panel layout needs custom styling for desktop/mobile.
* Filters must sync with parent view to reflect results in real time.
* Expected to be reused across sales module as well.

---

## 🧭 To-Do

* [ ] Implement `FilterPanelWrapper` container
* [ ] Group and align crop/plot/task filters
* [ ] Add reset (clear filters) button
* [ ] Ensure context-based filtering (per page)
