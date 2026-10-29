# MLBD assignments

Author: Ivana Stojanova (558296)

All notebooks are executed and saved with their outputs as requested, so they can be read without running them.

## Project structure
The project structre follows the requested layout:

- The two assigments(Recommender system and Deep Learning) in two different folders;
      - The Deep learning folder has models and results folders that were created from the experiments;
- The Readme.md, pyproject.toml, uv.lock and experiments.md in the root of the project;
- A data folder containing all the data

## How to run

1. In the project folder, create the environment by running `uv sync`. All dependencies are stored within the pyproject.toml file so they should install on your machine.
2. Start Jupyter and open a notebook, then run `uv run --with jupyter jupyter lab`, or open the folder in VS Code run all (or select a code cell) and select the `.venv` kernel.

### Running Assignment 2 again

Every training run is saved in a `results*/` JSON file. When the notebook is run again, finished runs are loaded instead of retrained, so Restart & Run All takes about a minute and shows all tables and graphs. The export, reload, confusion-matrix and visualisation cells use the saved models in `models/` and `models_cnn/`.

To retrain everything, delete the `results*`, `cv_result*.json` and the `models*` folders. Approximate training times on my laptop's CPU: Part 1 about 30 minutes plus about 10 minutes of cross-validation; Part 2 about 2.5 hours including the extras and cross-validation.

The reload cells at the end of both notebooks show how to use an exported model on data read from file:
- Part 1: `best_poker_model.keras` + `poker_test_hands.csv` (raw hands, same columns as `poker_hands.csv`)
- Part 2: `best_cnn_model.keras` + the PNG files listed in `cnn_test_files.csv`
