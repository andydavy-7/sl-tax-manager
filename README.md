# SL Personal Income Tax Manager

A free, open-source web app for calculating personal income tax in Sri Lanka for FY 2025/26 (Year of Assessment 2025/26). Built for individuals who need to reconcile APIT/PAYE withholdings across multiple employers, consultancy income, and bank interest.

**[Open the app →](https://andydavy-7.github.io/sl-tax-manager/)**

## Features

- **Multiple income sources** — track employment, consultancy, interest, and other income side by side
- **Monthly grid** — record income and tax withheld for each month (Apr–Mar)
- **Live calculation** — tax payable, slab-by-slab breakdown, and balance to pay update as you type
- **CSV bulk import** — populate sources from a spreadsheet in one go (template included)
- **JSON export/import** — back up your data or move between browsers
- **100% client-side** — your data never leaves your browser; nothing sent to any server
- **Mobile-friendly** — works on phones with a sticky bottom balance bar

## Sri Lanka FY 2025/26 tax slabs (built in)

| Annual Band | Rate |
|---|---|
| First 1,800,000 | 0% (personal relief) |
| Next 1,000,000 | 6% |
| Next 500,000 | 18% |
| Next 500,000 | 24% |
| Next 500,000 | 30% |
| Above 4,300,000 | 36% |

Personal relief is configurable in the app if rules change.

## How to use

1. Open the app
2. Click **Add Source** for each income stream
3. Enter monthly income and (if your employer/bank withheld tax) the tax deducted
4. Watch the **Slab Breakdown** and **Reconciliation** cards update live
5. Use **Export** to save a JSON backup

### Bulk import via CSV

1. Click **Download Template** to get a sample CSV
2. Fill in your data in any spreadsheet app
3. Click **Upload CSV** to import

The CSV format is `source_name,type,month,income,tax_deducted,tax_withheld_at_source`.

## Privacy

All calculations happen in your browser. Data is stored only in your browser's `localStorage`. No analytics, no tracking, no backend. View the source — it's a single HTML file.

## Tech

- Single `index.html`, no build step
- Vanilla JavaScript
- JetBrains Mono (via Google Fonts)
- Lucide icons (inline SVG)
- LocalStorage for persistence

## Disclaimer

This tool is for personal estimation only. Verify all figures with a registered tax consultant or the Inland Revenue Department (IRD) of Sri Lanka before filing.

## License

MIT — see [LICENSE](LICENSE).
