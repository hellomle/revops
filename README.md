# Intro RevOps + TalentOps Dashboard

This is the editable app-style version of the dashboard.

## Files

- `index.html` - page structure
- `styles.css` - visual styling and layout
- `app.js` - data loading, filters, charts, KPIs, and tables
- `data/default/bookings.csv` - default bookings data
- `data/default/talent.csv` - default talent master data
- `data/default/waitlist.csv` - default waitlist data

## How to run locally

Open a terminal in this folder and run:

```bash
python -m http.server 8000
```

Then open:

```
http://localhost:8000
```

The app also has embedded fallback data, but using a local server lets it read the CSV files from `data/default/`.

## Updating data

You can update data in two ways:

1. Replace the files in `data/default/`.
2. Use the in-page Data Manager to upload `bookings.csv`, `talent.csv`, or `waitlist.csv`.

Uploaded CSVs are stored in the browser and override the defaults until you click `Reset to default data`.
