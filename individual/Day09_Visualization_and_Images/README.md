# Day 9: Data Visualization and Multimodal Data; Working with Images

**Thursday 8 October 2026** · Instructors: Dr. Deepak Mishra, Krishnendhu, Zoya Fatima

## Schedule slot

Data Visualization and Multimodal Data (Matplotlib, Seaborn, charts and graphical interpretation); Working with Images and Multiple Data Types (Pillow, image properties, text/CSV plus image integration); hands-on: analytical plots, image processing.

## Files in this folder

| File | What it is | Type | Where it appears in the combined files |
|---|---|---|---|
| `Data_Visualization_and_Multimodal_Data_Slides.pdf` | 45 pages: Matplotlib, chart types, Seaborn, multimodal data, interpretation and best practice. The cover is dated 7 October 2026. | PDF slides | Slides section, Day 9 |
| `Matplotlib_Tutorial_FIFA_and_Gas_Prices.ipynb` | Matplotlib tutorial using the FIFA and gas-price datasets (19 cells). **Needs `fifa_data.csv` and `gas_prices.csv` in the same folder** (copy them from `datasets/`). | Notebook | Notebook section, Day 9 |
| `Matplotlib_Tutorial_30_Minutes.ipynb` | "Learn Matplotlib in 30 Minutes": figures and axes, line, scatter, bar, histogram, subplots, pandas, annotation, styles, pie charts, saving. This original file keeps its saved outputs (about 1.7 MB). | Notebook | Notebook section, Day 9 |
| `Hands_on_Data_Visualization_Student.ipynb` | Hands-on session with Tasks 1 to 13 and beyond (lists, tables, CSV, line, bar, scatter, box plot, heatmap, Seaborn). Optionally uses `tips.csv` from `datasets/`, or `sns.load_dataset("tips")` if online. | Notebook | Notebook section, Day 9 |
| `Images_Pillow_Theory_Slides.pdf` | 42 pages. Images and Multiple Data Types: Pillow and image properties (Mr. Jayakumar T V). Note: the PDF includes animation steps, so it has more pages than slides. | PDF slides | Slides section, Day 9 |
| `Images_Pillow_Lab_Slides.pdf` | 13 pages. Lab: build a picture, read its pixels, transform it (Mr. Jayakumar T V). | PDF slides | Slides section, Day 9 |
| `Images_Pillow_Lab_Exercise.ipynb` | Short Pillow lab notebook (9 cells). | Notebook | Notebook section, Day 9 |

## Notes

- **Known issue in the FIFA tutorial:** two cells use `.count()[0]`, which fails with a KeyError on current pandas (version 2 and later). Replace `[0]` with `.iloc[0]`. The files are unchanged from the original.

[Back to the main README](../../README.md)
