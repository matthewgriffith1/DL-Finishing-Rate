# DL-Finishing-Rate

# Pressure to Sack Rate: Quantifying DL Finishing Ability
### NFL Big Data Bowl 2023 | Baltimore Ravens Technical Assessment

## Overview

This project evaluates pass rush finishing ability using the Pressure-to-Sack Rate
(PTSR) metric, the defensive mirror of the quarterback Pressure-to-Sack ratio
familiar to NFL analysts. Where QB P2S% measures how often a quarterback escapes
pressure without being sacked, PTSR measures how often a pass rusher converts a won
rep into a sack. Using Weeks 1 through 9 of the 2022 NFL season from the NFL Big
Data Bowl dataset, this project identifies which pass rushers are the most efficient
finishers and examines whether finishing ability is related to how quickly defenders
generate pressure.

## Prerequisites

- R (>= 4.1)
- RStudio (recommended)
- Access to the NFL Big Data Bowl 2023 data via Kaggle or Onedrive

## Setup

1. Clone the repository
```bash
git clone https://github.com/[your-username]/dl-finishing-rate.git
cd dl-finishing-rate
```

2. Download the NFL Big Data Bowl 2023 dataset from Kaggle/Onedrive

Place all CSV files in the `data/` folder. See `data/README.md` for details.

3. Restore the R package environment
```r
renv::restore()
```

4. Open `analysis/dl_finishing_rate.Rmd` in RStudio and knit to HTML

## Viewing the Report

The pre-knitted HTML report is available at `outputs/dl_finishing_rate.html` and can
be opened directly in any browser without running R.

## Repository Structure

```
dl-finishing-rate/
|
|-- data/
|   |-- README.md
|
|-- analysis/
|   |-- dl_finishing_rate.Rmd
|
|-- outputs/
|   |-- dl_finishing_rate.html
|
|-- executive_summary/
|   |-- executive_summary.pdf
|
|-- technical_document/
|   |-- technical_document.pdf
|
|-- renv.lock
|-- .gitignore
|-- README.md
```

## Packages

- tidyverse
- ggplot2
- knitr
- gt
- gtExtras
- glue
- nflreadr
- ggrepel
