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
| Analysis and interpretation | | ○ | ● |
| Dashboard (`app.py`) | ● | ○ | |
| Presentation deck | ● | ○ | ○ |
| Repository organisation and review | ● | ○ | ○ |

Use ● for main responsibility and ○ for support.

## Ma Tianjiao

- **Topic and data:** chose the topic, found the HDB resale dataset and the MRT and block-location sources, and built the pipeline in `src/` (download, block locations, geocoding, cleaning, summary tables) with help from Claude (see AI_USAGE.md).
- **Dashboard:** built the Streamlit dashboard (`app.py`) with help from Claude and revised it after feedback from the TA (MRT and CBD distance, map, regression, "Help me choose") and the instructor (price per sqm by default, "Compare similar flats only", excluding the incomplete year 2026, reporting both % and S$ change, and the "About & method" tab).
- **Coordination and review:** set up the GitHub repository, split the tasks, reviewed and merged pull requests from Sun Jiayi, and deployed the dashboard on Streamlit Community Cloud.
- **Presentation:** drafted the slide deck with help from Claude (see AI_USAGE.md).


## Sun Jiayi

- **Dashboard refinement:** revised `app.py` to clarify dashboard logic and improve user-facing English. Updated titles to present data-driven conclusions that respond to dashboard selections, and polished explanatory text, chart labels, and other interface copy.
- **Documentation and consistency checks:** reviewed the dashboard against the project documentation, revised Markdown files including `CONTRIBUTIONS.md` and `AI_USAGE.md`, and checked that descriptions of the methods and findings remained consistent with the dashboard and README.
- **Presentation:** prepared supporting presentation materials and presented slides 4–6 and 10.

## Deng Shenbojia

- **Figures:** created `src/make_figures.py` (with help from Claude, see AI_USAGE.md), which draws 11 charts in `outputs/figures/`: 7 with Matplotlib (price trend, town growth by % and S$, million-dollar flats, MRT distance, regression effects, price map) and 4 with Seaborn to show distributions (histogram + KDE, box plot by town, 2019 vs 2025 side by side, and a regression plot of MRT distance vs price with its correlation), using the same definitions as `make_tables.py`, and added them to the README.
- **Interpretation:** rewrote the README's *Key findings* and *Limitations* in plain language, including why % and S$ rankings differ, why flats near the MRT cost more, and how the limitations affect our conclusions.
- **Dashboard screenshots:** took 6 screenshots of the main dashboard tabs (`outputs/figures/dashboard_*.png`) for the README and the presentation, choosing settings so the numbers match the README; while checking them, found and fixed an outdated number in the README (15 towns within budget, not 11).
- **Presentation:** presents slides 7–8 and 11–12. Also checked the deck against the dashboard and README and updated it: new dashboard screenshots, the Seaborn distribution chart on slide 6, a conclusion-style title for the town-growth chart, and consistent wording on slides 3, 8 and 12.

## How we worked together

- One shared GitHub repository; each member worked on their own branch and opened pull requests. Ma Tianjiao reviewed and merged the pull requests from Sun Jiayi. Deng Shenbojia merged his own pull requests, and Ma Tianjiao merged her own documentation pull request (#8), without a separate review.
- We held weekly meetings on Mondays to set our work plan for the week, and used a group chat to discuss and adjust the details.
