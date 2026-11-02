# Contributions

This project was completed as group work for **DS608 Data Analytics for Economics** (SMU, MSc in Data Science) by three students.

> Contributions are summarised below based on each member’s work on the project.

## Summary

| Area | Ma Tianjiao | Sun Jiayi | Deng Shenbojia |
|---|---|---|---|
| Topic and proposal | ● | ○ | ○ |
| Data download and documentation | ● | | |
| Data cleaning (`src/wrangle.py`) | ● | | |
| Location data (MRT, geocoding) | ● | | |
| Analysis and interpretation | | | ● |
| Dashboard (`app.py`) | ● | ○ | |
| Presentation deck | | ● | ○ |
| Repository organisation and review | ● | ○ | ○ |

Use ● for main responsibility and ○ for support.

## Ma Tianjiao

- Found the HDB dataset and wrote the download and cleaning scripts; built the first version of the dashboard; added MRT distance and the map after TA feedback.
- Coordinated the shared GitHub workflow, keeping project code, data documentation, analysis outputs, and presentation materials organised. Helped review changes submitted through branches and pull requests before they were merged into `main`.


## Sun Jiayi

- Refining `app.py`, including clarifying dashboard logic and polishing the English wording of titles, explanatory text, and chart labels.
- Reviewing and updating the dashboard and project Markdown files to keep their descriptions, methods, and findings consistent.
- Preparing the PowerPoint presentation and supporting presentation materials.

## Deng Shenbojia

- **Figures:** created `src/make_figures.py` (with help from Claude, see AI_USAGE.md), which draws 11 charts in `outputs/figures/`: 7 with Matplotlib (price trend, town growth by % and S$, million-dollar flats, MRT distance, regression effects, price map) and 4 with Seaborn to show distributions (histogram + KDE, box plot by town, 2019 vs 2025 side by side, and a regression plot of MRT distance vs price with its correlation), using the same definitions as `make_tables.py`, and added them to the README.
- **Interpretation:** rewrote the README's *Key findings* and *Limitations* in plain language, including why % and S$ rankings differ, why flats near the MRT cost more, and how the limitations affect our conclusions.
- **Dashboard screenshots:** took 6 screenshots of the main dashboard tabs (`outputs/figures/dashboard_*.png`) for the README and the presentation, choosing settings so the numbers match the README; while checking them, found and fixed an outdated number in the README (15 towns within budget, not 11).
- **Presentation:** _to be added once the group has split the slides._

## How we worked together

- One shared GitHub repository; each member worked on their own branch and opened pull requests, which another member reviewed before merging into `main`.
- We held weekly meetings on Mondays to set our work plan for the week, and used a group chat to discuss and adjust the details.

## Personal portfolio statement (template)

> This project was completed as part of DS608: Data Analytics for Economics in a group of 3 students. My main contributions were [specific tasks], with particular responsibility for [brief detail]. I also contributed to [secondary task], helped prepare the final presentation, and reviewed the GitHub repository to ensure that the project was clearly documented and reproducible.
