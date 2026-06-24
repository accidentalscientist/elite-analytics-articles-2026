# Elite Analytics Articles 2026

Ten long-form, evidence-led articles curated from the Accidental Scientist daily analytics collections. The collection is designed for a reader-facing website and a reproducible technical portfolio.

## Collection

- Seven energy-transition articles: Australian electricity, the NEM, global renewables, climate evidence, emissions, and demand.
- Three broader articles: graduate outcomes, urban inequality, and overlooked economic leaders.

Each article includes a concise editorial narrative, an argument to lead with, a figure brief, and links to the source notebooks. The original notebooks remain the evidence trail; this repository is the polished publication layer.

## Local website test

From the Django project root, run:

```powershell
.\venv\Scripts\python.exe manage.py import_elite_articles --publish
.\venv\Scripts\python.exe manage.py runserver
```

The importer creates or updates posts from `articles/`. `--publish` is for local review; omit it to load the collection as drafts.

## Before public release

Export the named figure from each source notebook, add it through Django admin as the post image, and add any supporting figures using the BlogImage inline. Check data dates and source links again before publishing.

## Source collections

- [May 2025](https://github.com/accidentalscientist/daily-data-analytics-may2025)
- [June 2025](https://github.com/accidentalscientist/daily_data_analytics_june2025)
- [July 2025](https://github.com/accidentalscientist/daily_data_analytics_july2025)
- [August 2025](https://github.com/accidentalscientist/daily_data_analytics_august2025)
