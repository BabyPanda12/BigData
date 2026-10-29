# Datasets

All datasets are included in this folder; nothing has to be downloaded.

| Folder / file | Used by | Source |
|---|---|---|
| `movielens/` | `01_recommender_system/` | MovieLens `ml-latest-small` (GroupLens, <http://grouplens.org/datasets/>) plus `imdbdata.json`, provided with the course. See `movielens/README.txt` for the licence. |
| `poker_hands.csv` | `02_deep_learning/neural_network.ipynb` | Course file *poker_hands.csv* (MLBD Assignment 2, Brightspace). 1,025,010 hands, columns `suit1, rank1, ..., suit5, rank5, ranking`. |
| `letters/` | `02_deep_learning/convolutional_network.ipynb` | Glagolitic letter set created for *Introduction to Machine Learning*: 1,286 PNGs (128x128 RGBA), named `<letter>_<date>_<time>_<id>.png`. |

The notebooks use relative paths (`../data/...`), so run them from their own folder (the default in Jupyter and VS Code).
