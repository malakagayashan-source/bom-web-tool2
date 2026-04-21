# BOM Database Web Tool

A fully self-contained, single-file web application for browsing and consolidating Bill of Materials (BOM) data from your Excel database — no server required.

## Features

- **Product Search** — Instantly search across 4,316 products by code or name
- **Multi-Product Selection** — Add multiple products with individual quantities
- **BOM View** — Card-based visual overview of each product's components
- **BOM Detail Table** — Full flat table of all parts across selected products
- **Consolidated Parts Table** — Aggregated totals for all unique parts across all selected products (quantities scaled by your chosen quantities)
- **CSV Export** — Download the consolidated parts list as a CSV file

## How to Use

1. Open `bom_app.html` in any modern web browser (Chrome, Firefox, Edge, Safari)
2. Search for a product by code or name in the left sidebar
3. Set the quantity and click **+ Add**
4. Repeat for as many products as needed
5. Click **Generate BOM**
6. View the BOM cards, detail table, and consolidated parts
7. Export to CSV if needed

## Deploy to GitHub Pages

1. Create a new GitHub repository
2. Upload `bom_app.html` to the repository root
3. Rename it to `index.html` (optional, for cleaner URL)
4. Go to **Settings → Pages**
5. Set Source to `main` branch, root folder
6. Your app will be live at `https://yourusername.github.io/your-repo-name/`

## File Structure

```
/
└── bom_app.html    ← Entire application (self-contained, ~2.5 MB)
└── README.md
```

All BOM data is embedded directly in the HTML file — no database, no API, no backend needed.

## Technical Notes

- Pure HTML + CSS + Vanilla JavaScript — zero dependencies
- All 4,316 products and their BOM lines are embedded as JSON
- Search is client-side with real-time filtering
- Works offline after initial load
