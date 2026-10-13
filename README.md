# MATH 261A Project 1

**Author:** Xinyi Xu  
**Submission date:** October 12, 2026  
**Repository:** <https://github.com/XinyiXu0218/math261a-project1>

## Project description

This project uses simple linear regression to study the tract-level association between annual mean PM2.5 concentration and age-adjusted asthma emergency department visit rates across California census tracts using CalEnviroScreen 5.0.

## Repository structure

- `project1_version2.qmd` — Quarto source for the analysis and paper.
- `project1_version2.pdf` — rendered report submitted for the project.
- `references.bib` — BibTeX references for data, literature, R, R packages, and Quarto.
- `README.md` — project description, data-source information, and reproducibility notes.
- `.gitignore` — prevents external raw data and local R/Quarto files from being committed.
- `data/` — optional local location for the downloaded CalEnviroScreen CSV; this folder is ignored by Git.

## Data source

The data are from **CalEnviroScreen 5.0**, published by the California Office of Environmental Health Hazard Assessment (OEHHA) and distributed through the California Open Data Portal.

Data page: <https://data.ca.gov/dataset/calenviroscreen-5-0>

The metadata supplied with the dataset identifies the public access level as public, states that there are no restrictions on public use, and lists the license field as not specified. The raw external data are not included in this repository. When rendered, the Quarto file first looks for a local copy of the CSV and otherwise attempts to read the official California Open Data download.

## Reproducibility

The analysis is written in R and uses `tidyverse`, `ggpubr`, `patchwork`, and `knitr`. The report is rendered with Quarto. The statistical model, summary statistics, coefficient table, figures, and numerical values reported in the text are generated from code in the Quarto file.

To reproduce the report, open `project1_version2.qmd` in RStudio and render it to PDF. A local copy of the data may be stored at `data/calenviroscreen50_070126.csv`; because `data/` is ignored by Git, that external raw file will not be committed.

## External resources and LLM use

External resources were used in preparing this project. OEHHA documentation and the cited scholarly literature were used for background, data definitions, and methodological context. ChatGPT was used to assist with organizing the Quarto document, checking code structure, and editing wording. The author reviewed the statistical analysis, numerical results, interpretation, citations, and final written report before submission.