# Spotify genre analysis (P4DS coursework)

A data analysis of around 170,000 Spotify songs from 1921 to 2020, with a
simple genre recommender built on top. Group coursework for a Programming
for Data Science module (Leeds, 2020), with two classmates.

## At a glance

- **Problem:** how do musical genres relate to each other, and which genres
  sound most alike?
- **Data:** a Spotify song dataset with 19 features per track, including
  danceability, energy, valence, tempo, acousticness and popularity. The
  full file (`data.csv`) is included, along with genre and artist summaries.
- **Method:** pandas for cleaning and aggregation, matplotlib for charts,
  and a distance-based recommender for genres.
- **Stack:** Python, pandas, matplotlib, Jupyter.

## What's in the repo

| File | What it is |
|---|---|
| `data.csv` | Track-level data: one row per song |
| `data_by_genres.csv`, `data_by_artist.csv`, `data_by_year.csv` | Averaged summaries |
| `data_w_genres.csv` | Tracks joined with their genre labels |
| `Genre_Recommendations.ipynb` | Recommends similar genres. Users pick a genre and a comparison metric, and the notebook finds the closest genres by Euclidean distance over normalised features |
| `Genres_by_artist_EB.ipynb` | Looks up the genres associated with an artist |
| `A3_Data_Analysis_Project.ipynb` | The assignment notebook (see known gaps) |
| `Visualisation1EB.ipynb`, `Sian's Notebook.ipynb` | Additional analysis and charts |
| `genreComparison.png`, `genre_recs_from_genre.png`, `genre_recs_from_artist.png` | Output charts |
| `perfectuse1.png`, `imperfectuse1.png` and related | Charts comparing well and poorly structured visualisations |

## How to run

```bash
pip install pandas matplotlib jupyter
jupyter notebook Genre_Recommendations.ipynb
```

Run the cells from the top. The recommender asks for a genre, the number of
results, and the metric to compare by.

## Known gaps

- `A3_Data_Analysis_Project.ipynb` still contains template text (for
  example "_Project Title_" and the example fridge-magnet cells). It needs
  to be replaced with the group's own write-up.
- The assignment notebook lists the group's university email addresses.
  Remove them before sharing the repository more widely.
- `data.csv` is about 29 MB. GitHub accepts it, but it's close to the size
  where Git LFS becomes worth considering.

## Data

Check the dataset's licence terms before reusing the data outside this
coursework.
