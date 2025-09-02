# 💰 Sales Management – Frontend Plan

This section outlines the breakdown of all **pages**, **components**, and **estimated times** for building the **Sales Management** module. The module includes multiple views depending on filters applied (Clients / Crops) and temporal scope (short-term vs long-term).

Each view includes a forecasted grid, interactive insights, and togglable indicators. Implementation is organized by page, with reused components noted.

---

## 🔗 Pages

* [Crop-Forecast View (Short-Term)](./sales-crop-short-term.md)
* [Crop-Forecast View (Long-Term)](./sales-crop-long-term.md)
* [Client-Forecast View (Short-Term)](./sales-client-short-term.md)
* [Client-Forecast View (Long-Term)](./sales-client-long-term.md)
* [Sales Simulator Modal](./sales-simulator.md)

---

## 🔁 Shared Components

* [Filters (Crops, Orders, Promotions)](./filters.md)
* [Toggle Indicators Bar](./shared-components.md)
* [Shared UI Components](./shared-components.md)

---

## 🧩 Filters & Toggles

| Filter Group    | Filter Options                                                                             | Component Type         | Inherited? | Notes                     |
| --------------- | ------------------------------------------------------------------------------------------ | ---------------------- | ---------- | ------------------------- |
| **Filter By**   | Crops, Orders, Promotions                                                                  | `Dropdown`             | ✅ Yes      | Shared dropdown component |
| **Toggle Show** | Confirmed, Potential, Expected Orders, Quantity, Revenue, Promotion, Crop Mix, Channel Mix | `Indicator Toggle Bar` | ✅ Yes      | Used across all views     |

---

## 📅 Timeline Summary

| Page                         | Est. Time (hrs) | Status        | Expected End Date |
| ---------------------------- | --------------- | ------------- | ----------------- |
| Crop Forecast (Short-Term)   | 8               | ⬜ Not Started |                   |
| Crop Forecast (Long-Term)    | 7.5             | ⬜ Not Started |                   |
| Client Forecast (Short-Term) | 8               | ⬜ Not Started |                   |
| Client Forecast (Long-Term)  | 7.5             | ⬜ Not Started |                   |
| Sales Simulator Modal        | 6               | ⬜ Not Started |                   |

---

## 🧭 Next Steps

* Create individual markdowns per sales view and simulator modal
* Cross-check shared components from general UI and production
* Begin breakdown of component-level estimates per page
