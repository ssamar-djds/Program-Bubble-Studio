# Program Bubble Studio

A browser tool for turning an architectural space program into to-scale bubble diagrams, packed print sheets, and an adjacency diagram.

Open `index.html` in any modern browser — no install or build step.

## What it does

- **Program** – Load a program from Excel/CSV, or type spaces in directly. Edit names, square footage, colors, and relationships in a table, and export the program back to Excel.
- **Bubbles & print sheets** – Each bubble's area equals the space's square footage, drawn at a chosen architectural or engineering scale (1/32" to 1/4" = 1'-0", 1" = 10' to 1" = 100'). Bubbles are packed tightly onto 11×17 (or other) sheets to use as little paper as possible. Download as a to-scale PDF with a scale bar on every sheet — print at **Actual size / 100%**.
- **Adjacency diagram** – Solid lines for direct access, dashed lines for close-to. Auto-arranges bubbles so related spaces sit together with few crossing lines. Drag bubbles, and connect or disconnect spaces by clicking; changes update the program table. Download as PDF, to scale or fitted to the sheet.

## Excel format

| Space Name | Square Feet | Direct Access | Close To |
|---|---|---|---|
| Lobby | 600 | Community Room | Offices |
| Community Room | 1800 | Lobby, Kitchen | Storage |

List related spaces by name, separated by commas. A blank template can be downloaded from the Program tab.

## Notes

- Your work is saved in your own browser (localStorage); it isn't shared between people or devices. Use "Export program to Excel" to keep or share a program.
- Uses [SheetJS](https://sheetjs.com/) for Excel and [jsPDF](https://github.com/parallax/jsPDF) for PDFs, loaded from cdnjs.
