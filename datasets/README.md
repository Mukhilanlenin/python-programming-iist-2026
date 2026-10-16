# Datasets

Small data files used by the notebooks.

| File | Rows | Used by | Notes |
|---|---|---|---|
| `fifa_data.csv` | about 18,200 | Day 9, Matplotlib tutorial (FIFA and gas prices) | FIFA player data (9 MB) |
| `gas_prices.csv` | 19 | Day 9, Matplotlib tutorial (FIFA and gas prices) | Gas prices by country and year, 1990 onwards |
| `tips.csv` | 244 | Day 9, hands-on data visualization (optional) | Restaurant bill and tip data. The notebook can also load this from Seaborn with `sns.load_dataset("tips")` when online |

**Using them.** The combined notebook (`combined/Python_Programming_Complete_Notebook.ipynb`) reads these files from `../datasets/`, so it works as long as the folder layout is kept. The individual notebooks in `individual/` are unchanged originals and expect the file to sit next to the notebook, so copy the CSV into the notebook's folder first.

The Day 8 notebooks need no data file: they create their own sample data.

[Back to the main README](../README.md)
