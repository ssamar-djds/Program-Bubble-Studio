# Program Bubble Studio

A browser tool for turning an architectural space program into to-scale bubble diagrams, packed print sheets, and an adjacency diagram.

Open `index.html` in any modern browser — no install or build step. Click "Load office example" to see a finished diagram.

## What it does

- **Program** – Load a program from Excel/CSV, or type spaces in directly (with a quantity for repeated rooms). Edit names, square footage, relationships, icons, clusters, color groups and notes in a table (or the copy under the adjacency diagram), select several rows to change them at once, and export the program back to Excel.
- **Bubbles & print sheets** – Each bubble's area equals the space's square footage, drawn at a chosen architectural or engineering scale (1/32" to 1/4" = 1'-0", 1" = 10' to 1" = 100'). Bubbles are packed tightly onto 11×17 (or other) sheets to use as little paper as possible. Download as a to-scale PDF with a scale bar on every sheet — print at **Actual size / 100%**.
- **Adjacency diagram** – Solid lines for direct access, dashed lines for close-to. Arrange automatically, or around a hub space with its connections spread evenly. Drag bubbles, connect or disconnect spaces by clicking, and add icons or cluster membership by clicking; changes update the program table. Download as PDF, to scale or fitted to the sheet.
- **Clusters** – Group repeated or related spaces. Shown as a soft filled shape, a dotted outline, or both; set a grid (rows × columns) per cluster. Link a space to a cluster's name to draw one line to the whole group.
- **Color groups** – Color spaces by color group (e.g. Work, Support, Building), with one editable color per group.
- **Icons** – Acoustic, Privacy, Nature and Sunlight markers on the edge of each bubble, with a legend in the bottom-right corner.

## Excel format

| Space Name | Square Feet | Direct Access | Close To | Icons | Cluster | Color Group | Notes | Quantity |
|---|---|---|---|---|---|---|---|---|
| Open Office | 1500 | Private Offices, Med. Meeting Rm | | Sunlight | | Work | (10 ppl) | 1 |
| Private Office | 150 | | | Privacy | Private Offices | Work | | 10 |

Only the first two columns are required. List related spaces (or cluster names) separated by commas. A filled-in template can be downloaded from the Program tab.

## Notes

- Your work is saved in your own browser (localStorage); it isn't shared between people or devices. Use "Export program to Excel" to keep or share a program.
- Uses [SheetJS](https://sheetjs.com/) for Excel and [jsPDF](https://github.com/parallax/jsPDF) for PDFs, loaded from cdnjs.
