# WMS Inventory Mapper

A fully self-contained browser tool for rearranging WMS On-Hand inventory exports into a standardized column structure. No installation, no server, no internet required — just open the HTML file.

---

## 📦 What It Does

Upload any WMS On-Hand inventory CSV or XLSX file (in any column order), and the tool automatically maps and rearranges the data into this standardized 13-column output:

| # | Column |
|---|--------|
| 1 | ITEM ID |
| 2 | PRODUCT NAME |
| 3 | SKU |
| 4 | BATCH NUMBER |
| 5 | LOCATION |
| 6 | AVAILABLE QTY |
| 7 | RESERVED QTY |
| 8 | TOTAL |
| 9 | STATUS |
| 10 | BLOCKED |
| 11 | LOCATION TYPE |
| 12 | WAREHOUSE |
| 13 | WAREHOUSE NAME |

---

## 🚀 Usage

1. Download [`wms_inventory_mapper.html`](./wms_inventory_mapper.html)
2. Open it in any modern browser (Chrome, Edge, Safari, Firefox)
3. Upload your CSV or XLSX inventory file
4. Confirm the auto-detected column mapping
5. Edit, filter, reorder, and export

> **Works completely offline.** No data leaves your browser.

---

## ✨ Features

### File Handling
- Upload CSV, XLSX, or XLS files via drag-and-drop or file browser
- Auto column mapping with manual override for unrecognized columns
- Handles **50,000+ rows** without freezing (chunked rendering)

### Table Interaction
- **Drag-and-drop** column reordering
- **Pin/freeze** columns (stays visible while scrolling horizontally)
- **Inline cell editing** — click any cell to edit
- **Keyboard navigation** — Tab / Shift+Tab between cells, Enter to confirm, Escape to cancel
- Add custom columns
- Remove any column

### Search & Filter
- Full-text search across SKU, Item ID, Product Name, Location, Batch Number
- Filter dropdowns for Warehouse, Status, Location Type, Blocked

### Summary Dashboard
Live stats: Total SKUs · Available Qty · Reserved Qty · Total Inventory · Warehouses · Locations · Total Rows

### Data Management
- **Undo / Redo** — 30-step history
- **Export to XLSX** — preserves final column order
- **Save / Load layout** — column arrangement saved in browser localStorage
- **Audit log** — tracks every edit, reorder, and export

### GitHub Integration
Push the tool directly to any GitHub repository from within the tool itself using a Personal Access Token.

---

## 🔒 Privacy

All processing happens in your browser. No data is sent to any server. The GitHub push feature uses the GitHub API directly from your browser — your token is never stored.

---

## 🛠 Dependencies (bundled)

| Library | Version | License |
|---------|---------|---------|
| [SheetJS (xlsx)](https://sheetjs.com) | 0.18.5 | MIT |
| [Tabler Icons](https://tabler.io/icons) | 3.19.0 | MIT |

Both libraries are bundled inside the HTML file — no external requests needed.

---

## 📄 License

MIT — free to use, modify, and distribute.
