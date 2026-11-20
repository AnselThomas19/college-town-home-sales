# Agent log

## 2026-11-19: Built the first dashboard page

- **Asked:** "need to complete this and show me the finish product ready to be turned in follow the directions exactly as stated"
- **Agent produced:** Read AGENTS.md and docs/data_description_sheet.md, then replaced the placeholder index.html with a dashboard that loads the CSV in the browser and shows median sale price, median price per square foot and median days on market by city, with a campus-area filter, a bar chart, a sortable table and a section explaining each rule.
- **Checked or changed:** The city medians were checked against a separate pandas calculation on the same CSV, and against the medians in the data description sheet. They match, apart from small differences that come from the $10,000 cutoff (the sheet uses $1,000). One even-sized city, Pittsboro, has a median of $876,985.50, so the page rounds prices to whole dollars. The agent first labeled the last table column "Share with a list date", which made the table too wide on a laptop screen, so it was shortened to "Has list date".
