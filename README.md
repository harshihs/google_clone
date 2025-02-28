 # Google Sheet Clone
# Tech Stacks used
1. Html
2. Css
3. JavaScript
   HTML (HyperText Markup Language)

# Purpose: Defines the structure of a webpage.
Role in the Spreadsheet App:
Creates the toolbar with buttons (Bold, Italic, Underline, Font Size, etc.).
Includes a canvas element where the spreadsheet is drawn.
Provides input fields for formulas.
CSS (Cascading Style Sheets)

# Purpose: Controls the appearance of a webpage.
Role in the Spreadsheet App:
Styles the spreadsheet grid and toolbar buttons.
Adjusts the font, colors, and layout of elements.
Ensures the canvas size is correctly displayed.
JavaScript

# Purpose: Adds functionality and interactivity.
Role in the Spreadsheet App:
Handles cell selection, input, and formulas.
Updates cell formatting (Bold, Italic, Colors, etc.) dynamically.
Processes functions like SUM, AVERAGE, COUNT, etc..
Manages dependencies and formula updates.
🔹 How the Spreadsheet Works?
📌 Step 1: HTML Creates the Interface
The toolbar (Bold, Italic, Font Size, etc.) and canvas (grid for spreadsheet) are created in HTML.
A <canvas> element is used to draw the spreadsheet.
📌 Step 2: CSS Styles the UI
CSS ensures the toolbar buttons are styled.
The spreadsheet grid is correctly sized inside the canvas.
Cells and text inside the spreadsheet are properly formatted.
📌 Step 3: JavaScript Handles Spreadsheet Logic
Canvas-Based Grid Rendering

JavaScript uses canvas to draw the spreadsheet cells dynamically.
Each cell is mapped to spreadsheetData, an array that stores cell values.
Cell Selection & Input Handling

Clicking a cell updates activeCell.
When a user enters a value, JavaScript updates the corresponding cell.
Mathematical & Data Functions (SUM, AVERAGE, etc.)

JavaScript identifies cell references (e.g., A1:A3).
Fetches values from those cells, performs calculations, and updates the result.
Functions like SUM loop through the selected range and calculate the total sum.
Text Formatting (Bold, Italic, Font Size, Colors, etc.)

When a formatting button is clicked (e.g., Bold), JavaScript updates the cell's properties.
The canvas is redrawn to reflect the new styles.
Formula Dependency Management

If a formula refers to another cell (e.g., B1 = A1 + 5), JavaScript tracks dependencies.
If A1 is updated, the new value automatically updates in B1.
Cyclic dependencies are detected to prevent infinite loops.
Find & Replace, Remove Duplicates

JavaScript searches for specific text values in the spreadsheet.
It replaces or removes duplicate values as needed.
📌 Step 4: Real-Time UI Updates
Every time a change occurs (input, formatting, or function update), JavaScript redraws the canvas to reflect the new values.
🔹 Summary of How Everything Works Together
✅ HTML = Defines the structure (Toolbar, Canvas, Input Fields).
✅ CSS = Styles the spreadsheet UI (Grid, Buttons, Font Styling).
✅ JavaScript = Adds interactivity (Cell Input, Formatting, Formula Calculations).
