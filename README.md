# Lecture Notes 2026/27 – teaching support files

This public repository hosts the teaching support files for the 2026/27 sessions:
the student delivery notebooks, the student lab notebooks and the datasets they load.

## Keep the folder structure

Do not rename or move anything inside `2026-27/`. The notebooks look files up by
their exact path (for example `2026-27/datasets/owid_co2_cleaned.csv`).

## How the notebooks get their data

Each notebook that loads data starts with a setup cell. It uses a local copy if the
notebook runs inside a copy of this repository. Otherwise (for example in Google
Colab) it downloads the file once from the raw GitHub URL:

```
https://raw.githubusercontent.com/<FINAL_OWNER>/<FINAL_REPO>/main/2026-27/datasets/<file>
```

## Notebooks you were given before this repository existed

In the setup cell, replace the placeholder

```python
COURSE_REPO = "OWNER/REPO"
```

with

```python
COURSE_REPO = "<FINAL_OWNER>/<FINAL_REPO>"
```

Leave everything else unchanged, then run the cell again.

## Data licences

Each dataset keeps its source's licence (Open Government Licence v3.0, CC BY 4.0,
CC BY-SA 4.0, CC0, Copernicus Sentinel data terms or public domain).
`pokemon.csv` comes from the Kaggle dataset *Pokemon with stats* by Alberto Barradas (CC0: Public Domain). Credit the source
when you reuse a file.
