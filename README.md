# Physics Graph Studio — GitHub Pages edition

## Publish for your classes
1. Extract this ZIP on your computer.
2. Create a GitHub repository (use a public repository with GitHub Free).
3. Upload the extracted files and the entire `vendor` folder to the repository root. `index.html` must be at the top level, not inside another folder. Do not upload only the ZIP.
4. Open the repository’s **Settings → Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**, then **main** and **/(root)**. Click **Save**.
6. When deployment finishes, use the website link shown on the Pages settings screen. Share that link with students.

No npm installation, build command, API key, backend, or ChatGPT account is needed. All JavaScript dependencies are bundled. Relative file paths support GitHub project sites. The included `.nojekyll` file disables Jekyll processing; retain it if your file browser shows hidden files.

Official publishing instructions:
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Use the graphing tool
- Paste spreadsheet data into the four columns: x, x uncertainty, y, y uncertainty. Uncertainties accept absolute values or percentages; scientific notation is supported.
- Use **Graph settings** to edit title, quantities, units, symbols, axis limits, intervals and line endpoints.
- Use **Appearance** for individual text sizes or the overall text scale.
- Select maximum or minimum gradient in **Adjust line**, then drag a circle to rotate the line or drag its body to shift it. Crossing counts show how many uncertainty rectangles the line intersects.
- **Reset automatic fits** restores calculated lines. Editing the measurements also resets manual adjustments.
- **Save graph** defaults to A4 portrait, 2480 × 3508 pixels at 300 dpi. Landscape and custom dimensions are available. Exported PNGs have a white background and omit drag handles.
- **Desmos equations** provides copyable equations for the current three lines. Paste each equation into a separate Desmos expression.
- **Copy graph URL** includes the current data, labels and settings. Send this copied URL to share a particular graph. A normal website URL opens the recipient’s own saved work or sample data.
- Changes autosave locally in each browser. Undo/redo operates during the current page session. Autosave is not a server backup and does not synchronize across devices. Shared computers share browser-local saved state.

## Calculation notes
The original Beep Boop Machines ordinary least-squares fit, corner-search maximum/minimum gradient algorithm, numeric parsing and educational feedback are retained. The max/min search is heuristic: a returned limit is not guaranteed to intersect every uncertainty rectangle. Check the displayed crossing counts. Vertical regression is undefined when x values are all identical.

## Credits
Based on https://www.beepboopmachines.com/ with extended controls and export. Bundled third-party libraries include SlickGrid, jQuery, jQuery UI and Chart.js. Their existing source comments and license notices are retained. No new license is asserted for the upstream code.

Prepared 23 October 2026. The ZIP contains application files only, with no hosting credentials, account-specific configuration or student data.
