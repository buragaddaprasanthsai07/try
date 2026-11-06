# IMDb Movie Analytics Dashboard

Streamlit practical examination dashboard (Student: B prasanth Sai, PRN 250200203).

## Deployment checklist

1. Place your **original IMDb Top 250 Movies CSV** in this folder, alongside `app.py`.
   Do not rename its columns. Ensure the CSV is committed to GitHub.
2. Upload `app.py`, `requirements.txt`, `banner.png`, `README.md`, `.gitignore`, and the CSV to the root of your repository.
3. Streamlit Community Cloud: select your GitHub repository, `main` branch, and entrypoint `app.py`.
4. The app automatically finds the first relevant IMDb CSV in its own folder. The dashboard relies on title, genre, country, averageRating, numVotes and grossWorldwide columns.
5. If an old app is already deployed, push a commit to GitHub. Streamlit Cloud should rebuild when `requirements.txt` changes.

## Run locally

```powershell
python -m pip install -r requirements.txt
python -m streamlit run app.py
```

## Notes

- All charts have distinct Streamlit keys, including charts repeated in tabs.
- The movie explorer includes genre, countries, rating range, minimum votes, title, sort order, filtered table, and reset.
- The search form includes title, genre, minimum rating, and session-state selection.
- The page includes initial 10 rows, row and column count, data types, and missing-value checks.
- Metrics use the data in the CSV, so they will differ from reference screenshots if the dataset differs.
- No made-up dataset is included. You must add your real CSV before deploying.
