# 📊 Sales Simulator – Sales Module

This view simulates the **impact of price changes** on projected sales, inventory, and waste—per client group, crop, and channel.  
It enables data-driven pricing strategies by previewing trade-offs across **agricultural**, **environmental**, and **economic** dimensions.

---

![Sales Simulator](./images/sales-simulator.png)

---

## 🧩 Component Breakdown

| Component Name             | Page Used         | Inherited? (from Shared) | React Ready?                            | Needs Customization?                                   | Est. Time (hrs) | Priority | Status         | End Date |
|---------------------------|-------------------|--------------------------|-----------------------------------------|--------------------------------------------------------|------------------|----------|-----------------|----------|
| **Sidebar Navigation**     | All Pages         | ✅ Yes                    | ✅ Yes (shadcn/ui)                       | Already implemented                                    | —                | High     | ✅ Ready        |          |
| **Navbar – Top**           | All Pages         | ✅ Yes                    | ✅ Yes (shadcn/ui)                       | Already implemented                                    | —                | High     | ✅ Ready        |          |
| **Filter Pills**           | This Page         | ❌ No                     | ⚠️ Partial (Tag/Chips UI)               | Crop / Channel / Client group selection as pills       | 2                | High     | ⬜ Not Started  |          |
| **Price Slider**           | This Page         | ❌ No                     | ⚠️ Partial (Slider component)           | Range selection + marker on selected price             | 2.5              | High     | ⬜ Not Started  |          |
| **Simulated Bar Chart**    | This Page         | ❌ No                     | ❌ No                                    | 3-color segmented bar for sales, inventory, waste       | 3.5              | High     | ⬜ Not Started  |          |
| **Impact Icons (3 Pillars)**| This Page        | ❌ No                     | ✅ Yes (custom icon cards)              | Agriculture, Environment, Economy icons per row        | 1.5              | Medium   | ⬜ Not Started  |          |
| **Tooltip for Price Range**| This Page         | ✅ Yes                    | ✅ Yes (shadcn/ui Tooltip)               | Reused from general                                    | —                | Medium   | ✅ Ready        |          |
| **Week Display Block**     | This Page         | ✅ Yes                    | ✅ Yes                                   | Dates & week display                                  | —                | Medium   | ✅ Ready        |          |

---

## ⏱️ Total Estimated Time

| Component Type           | Description                                                | Time (hrs) |
|--------------------------|------------------------------------------------------------|------------|
| 🧩 **New Components**     | Filter tags, slider, chart, icons                          | **9.5 hrs** |
| ♻️ **Shared Components**  | Navbar, sidebar, tooltips, week labels                    | **~2 hrs** |
| ✅ **Total Combined Time**| Total for full page implementation                        | **11.5 hrs** |

---

## 📘 Notes

- This simulator is **modal-based** and launched from multiple entry points across Sales views.
- The **price slider** directly modifies the forecasted outcomes in real time.
- Each row includes simulation bars and **3 icons** for interpretation across impact types.
- Weeks shown are bound to forecast periods and adapt automatically.
- Mobile responsiveness is key due to the scrollable format and modal context.

---

## 🧭 To-Do

- [ ] Build price slider logic with thresholds
- [ ] Implement stacked bar chart with labels
- [ ] Bind crop/channel/client filters to forecast model
- [ ] Add icon-based insight block per week
