# 🧪 Production Management – Frontend Plan

This section documents all components, timelines, and breakdowns for the **Production Management** module of the Agricom platform.

---

## 🔗 Pages

Each page has its own markdown file containing:
- UI components (shared + unique)
- Time estimates per component
- Feature logic
- Status tracking

| Page Name | File |
|-----------|------|
| Weekly Production View | [weekly-view.md](./weekly-view.md) |
| Weather Forecast View | [weather-forecast.md](./weather-forecast.md) |
| Harvest Simulator | [harvest-simulator.md](./harvest-simulator.md) |
| Task Details Modal | [task-details-modal.md](./task-details-modal.md) |
| Filters Overview | [filters.md](./filters.md) |

---

## 🔁 Shared Components

These components are reused from the general UI layer.  
Reference: [shared-components.md](../general.md)

- Navbar
- Sidebar
- Dropdown (Select)
- Filter Panel
- Table/Grid Layout
- Tooltip
- Modal

---

## 📅 Timeline Summary

This table summarizes **estimated hours** to implement each production page and component. Ending dates will be filled once a start date is assigned.

| Page                     | Est. Time (hrs) | Status         | Expected End Date |
|--------------------------|------------------|------------------|--------------------|
| Weekly Production View   | 14.5             | ⬜ Not Started   |                    |
| Weather Forecast View    | 7                | ⬜ Not Started   |                    |
| Harvest Simulator        | 8                | ⬜ Not Started   |                    |
| Task Details Modal       | 6                | ⬜ Not Started   |                    |
| Filters (Dropdowns)      | 3                | ⬜ Not Started   |                    |

---

## 🛠️ To-Do

- [ ] Link to backend data sources
- [ ] Connect shared components with props
- [ ] Implement conditional views (weather)
- [ ] Track feature status in GitHub issues

