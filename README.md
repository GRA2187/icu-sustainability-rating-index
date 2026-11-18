<p align="center">
  <img src="logo.svg" alt="ICU Sustainability Rating Index logo" width="96">
</p>

<h1 align="center">ICU Sustainability Rating Index: Dashboard</h1>

<p align="center">
  A free, browser-based dashboard that rates how an intensive care unit (ICU) is doing on environmental sustainability.
</p>

<p align="center">
  <a href="https://YOUR-GITHUB-USERNAME.github.io/icu-sustainability-rating-index/"><strong>Open the dashboard</strong></a>
  &nbsp;&middot;&nbsp;
  <a href="ICU-Sustainability-Index-Dashboard-FAQ.pdf">Read the FAQ (PDF)</a>
  &nbsp;&middot;&nbsp;
  <a href="LICENSE">License</a>
</p>

> **Concept demo.** Every number on the page when it opens is SAMPLE data for a made-up ICU ("ICU A"). The items, weights and tier cut-offs are drafts for a working group to test, and none of them has been validated. Treat any result as a trial of the tool, not a rating of a unit.

## What the dashboard does

- **Checklist score and tier.** Turns a 19-item checklist into a score out of 100 and a tier: Getting started, Bronze, Silver, Gold or Platinum.
- **Core KPIs.** Shows five everyday items per ICU patient-day (gloves, isolation gowns, blood tests, chest X-rays and red bag waste), with their carbon in kg CO2e first and their cost beside it.
- **Going well, and what to work on.** Lists up to three of each, picked by fixed rules. No AI is involved.
- **CO2e saved today.** Shows the carbon and cost saved when the unit orders fewer blood tests or chest X-rays than the day before.
- **Staff commute (optional).** Two daily counts of how staff got to work.
- **Infection watch (not scored).** Infection rates the hospital already reports, typed in by hand, so the team can watch them while cutting waste. Lines that move together show an association, not a cause.
- **Tracking log.** Saves the page as one dated entry and shows the entries by day, week or month, with charts.
- **Export.** Saves a PDF summary and an Excel workbook of what is on screen.

## Who it is for

Everyone who works in the ICU:

| Role | How they use it |
| --- | --- |
| Physicians | Co-lead the unit's sustainability work and agree the checklist ratings with nursing |
| Nurses | Co-lead the ratings, lead bedside changes, and follow progress in the tracking log |
| Administrative staff | Gather and enter the numbers, keep the tracking log, and export and share reports |
| Infection prevention team | Enter the infection rates the hospital already reports |

The working group's view is that ICU clinicians should not have to collect or audit sustainability data. Administrative staff gather the numbers, and the physician and nurse leads agree the ratings.

## How to use it

1. Open the dashboard link. There is no login, no account and nothing to install. It works on a laptop, tablet or phone.
2. Look around the ICU A sample to see how each panel works. Tap any (i) icon for a plain-language definition and its source.
3. To assess your own unit, click **Start a blank assessment**, then fill in the checklist, the KPIs and any daily counts.
4. To track over time, open the **Tracking log** panel and click **Add this page's numbers to the log**. Next time, click **Continue from my last entry**.
5. Click **Export report** to save a PDF and an Excel file.

## Your data stays on your computer

- The page has no server, no database and no upload. What you type stays in your browser.
- Tracking log entries stay in the browser on the computer where you added them. Clearing the browser's data deletes them, so click **Download the log (CSV)** regularly and keep the file.
- Never type patient names, record numbers or any other patient identifiers. The tool only needs unit-level counts.

## How the score works

Each of the 19 items is rated G (green, full points), Y (yellow, half points), R (red, no points) or N/A (not applicable, drops out).

```
Score = 100 × (sum of points × rating value) ÷ (sum of points), over applicable items
```

| Tier | Score | Also needs |
| --- | --- | --- |
| Platinum | 90 to 100 | At least 3 core KPIs improved and held for 24 months |
| Gold | 75 to 89 | At least 2 core KPIs improved |
| Silver | 60 to 74 | Nothing extra |
| Bronze | 40 to 59 | Nothing extra |
| Getting started | Under 40 | Nothing extra |

Every tier also needs three prerequisites: named physician and nurse sustainability leads, at least 3 core KPIs measured for 12 months, and changes reviewed by quality and infection prevention. A KPI counts as improved when its latest rate is at least 10% below the unit's baseline. The FAQ explains every formula with a worked example.

## Use it offline

Download `index.html` and open it in a web browser. Everything the dashboard needs, including the PDF and Excel export tools, is inside that one file.

## Files in this repository

| File | What it is |
| --- | --- |
| `index.html` | The dashboard, in one self-contained file |
| `ICU-Sustainability-Index-Dashboard-FAQ.pdf` | Answers to common questions, with the formulas behind every number |
| `LICENSE` | The PolyForm Noncommercial License 1.0.0 and the required notice |
| `logo.svg` | The logo shown on this page |
| `README.md` | This page |

## Browser support

Tested in Google Chrome. The page uses standard web features found in current versions of Microsoft Edge, Safari and Firefox.

## Credits

**Built by Manideep Kanagala**, with guidance from **Dr Vinay Nadkarni** and **Dr Geethanjali Ramachandra**.

Built with care and a passion for saving lives. Dedicated to the tireless efforts of everyone in the ICU & Emergency Department.

## License

Freeware: free to use, and open to editing or modifying, for any noncommercial purpose under the [PolyForm Noncommercial License 1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0). The full terms are in [LICENSE](LICENSE).

Required Notice: Copyright (c) 2026 Manideep Kanagala

Commercial use is not covered by this license. Please contact Manideep Kanagala about any other use.

The dashboard includes three open-source libraries that keep their own MIT licenses: [jsPDF](https://github.com/parallax/jsPDF) 4.2.1, [jsPDF-AutoTable](https://github.com/simonbengtsson/jsPDF-AutoTable) 5.0.8 and [ExcelJS](https://github.com/exceljs/exceljs) 4.4.0.

## Feedback

Questions, ideas and corrections are welcome. Please open an issue in this repository or contact Manideep Kanagala.
