# AI Governance Dashboard

A prototype dashboard that shows AI tool usage, spend limits and unapproved ("Shadow AI") tools across an organisation. It is built for a CFO first, with the IT/security lead as the second reader.

It was made as an Associate Product Manager take-home assignment. **All figures are sample data for a fictional 1,000-person company.**

## What's on the page

| Part | Question | Answer in brief |
| --- | --- | --- |
| 1. The screen | Prototype one screen showing AI usage and spend limits | A CFO-first screen: what needs a decision, four key numbers, three charts, a Shadow AI table and a department filter. Rows open detail panels. |
| 2. The data | Which APIs and data sources would power it? | Vendor admin APIs (OpenAI, Anthropic, Microsoft Graph, GitHub) for spend and seats. Sign-in records, OAuth grants and expenses to find unapproved tools. The HR system for teams and leavers. |
| 3. Three charts | Which three charts, and why? | Spend vs limit by tool, spend trend with forecast, and seat utilisation. Each one leads to a decision. |

## How to use it

1. Change the **Department** filter and every number, chart and list updates.
2. Click any row marked **›** to open its details.
3. Yellow numbered boxes are **PM notes** explaining each decision. Hide them with the toggle.
4. Parts 2 and 3 are written out below the dashboard.

## Tech

A single static `index.html` with no build step and no dependencies. It uses plain HTML, CSS and JavaScript, and draws the charts in SVG. Fonts load from Google Fonts. It supports light and dark mode and phone widths.

Run it locally by opening `index.html` in a browser, or deploy the folder as a static site.
