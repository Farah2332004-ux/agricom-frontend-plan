# 🧩 Shared UI Components

> These components are reused across multiple sections (Farm Setup, Production, Sales).  
> Time estimates are based on whether ready-made React libraries (e.g. shadcn/ui, react-select, etc.) can be used or must be customized.

---

| Component Name          | Pages Used       | React Ready?                             | Needs Customization?                   | Est. Time (hrs) | Milestone | Priority | Status        | Expected End Date |
| ----------------------- | ---------------- | ---------------------------------------- | -------------------------------------- | --------------- | --------- | -------- | ------------- | ----------------- |
| Navbar – Top Navigation | All Pages        | ✅ Yes (shadcn/ui Navbar)                 | Minor layout overrides                 | 2               | Global    | High     | ⬜ Not Started |                   |
| Sidebar Navigation      | All Pages        | ✅ Yes (shadcn/ui Sidebar)                | Needs collapse logic                   | 2               | Global    | High     | ⬜ Not Started |                   |
| Sidebar Collapse Toggle | All Pages        | ✅ Yes (Button component)                 | Layout logic w/ context                | 1               | Global    | High     | ⬜ Not Started |                   |
| Dropdown – Generic      | All Pages        | ✅ Yes (react-select or shadcn/ui Select) | Needs variations (filter, async)       | 1.5             | M1        | High     | ⬜ Not Started |                   |
| Filter Panel            | All Filters      | ⚠️ Partial                               | Needs grouped filters & responsiveness | 3               | M1        | High     | ⬜ Not Started |                   |
| Date/Week Selector      | Prod, Sales      | ⚠️ Partial                               | Horizontal scroll, sticky weeks        | 3               | M2        | High     | ⬜ Not Started |                   |
| Table/Grid Layout       | Prod, Sales      | ⚠️ Partial (shadcn/ui Table)             | Needs sticky cols + virtual scroll     | 4               | M2        | High     | ⬜ Not Started |                   |
| Modal Window            | Task, Weather    | ✅ Yes (shadcn/ui Dialog)                 | Minor props config                     | 1               | M2        | Medium   | ⬜ Not Started |                   |
| Interactive Map         | Farm Setup       | ❌ No                                     | Use Leaflet/Mapbox w/ draw polygon     | 8               | M1        | High     | ⬜ Not Started |                   |
| Tabs / Toggle Panel     | Sales, Crop View | ✅ Yes (shadcn/ui Tabs)                   | Toggle logic for indicators            | 2.5             | M2        | Medium   | ⬜ Not Started |                   |
| Tooltip on Hover        | All pages        | ✅ Yes (shadcn/ui Tooltip)                | Dynamic data feed needed               | 1.5             | M2        | Medium   | ⬜ Not Started |                   |


---

## 📘 Notes

- ✅ = can be built almost instantly with libraries
- ⚠️ = partially reusable, needs moderate tweaks
- ❌ = fully custom logic, heavier lift
- ⬜ = Not Started (GitHub issues can be linked here)




