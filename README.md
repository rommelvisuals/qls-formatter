QLS Formatter
A browser-based tool for converting Shopify order exports to QLS shipping format. No installation, no backend — just open the HTML file and go.
What it does
Upload a Shopify CSV export, select which products to include, review the data, and download a clean XLSX file ready to import into QLS.
Features

Smart address parsing — splits street and house number using Shopify's invisible separator (U+2060), including bus/apartment numbers
Product filter — searchable, alphabetical chip filter with order counts per product
Preview table — search across order number, name, product, EAN, postcode, and more
Inline editing — click the edit icon on any row to fix missing data; Save or Undo to confirm
Missing data warnings — flags incomplete rows (street, house number, postcode, city, EAN, SKU) before you export
Shopify order links — click any row to open the order directly in Shopify admin
SKU/EAN as text — prevents scientific notation in Excel on long barcodes
Session persistence — auto-saves your work so accidental tab closes don't lose progress
Light and dark theme
Mobile responsive

Usage

Export orders from Shopify admin (Orders > Export > CSV)
Open qls-formatter.html in any browser
Drop the CSV file onto the upload area
Filter by product if needed
Fix any rows flagged under "Missing data"
Set a filename and click Download XLSX

Notes

Use the original Shopify CSV directly — do not open and re-save in Excel first, as Excel truncates long order IDs to scientific notation (1.23872E+13), which cannot be recovered
The store handle in the top bar (9a71d7-51) can be updated to match your Shopify store for correct order links

Tech
Plain HTML, CSS, and vanilla JavaScript. No frameworks, no dependencies except SheetJS (loaded via CDN) for XLSX export.

Developed by Rommel Salvatierra for Poopy
