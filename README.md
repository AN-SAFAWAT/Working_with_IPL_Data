# IPL Player Auction Analysis

## Overview

This repository contains the data analysis project for an IPL team's upcoming auction. The goal of the analysis is to identify top potential batters and all-rounders to strengthen the team's lineup. The dataset includes information on batsmen, bowlers, all-rounders, and wicket-keepers.

## Data Understanding

The structured dataset contains data of IPL players categorized into four types:

1. Batsman
2. Bowler
3. All-rounder
4. Wicket-keeper

Since the focus is on batters and all-rounders, the analysis does not require addressing data skewness but does require careful handling of outliers and null values.

## Problems and Solutions in Data

- **Outliers**: Uncapped players who have not debuted in the IPL are considered outliers and are removed from the analysis.
- **Players with Insufficient Data**: Players who have played fewer than 10 matches and have null data entries are also removed.
- **Null Value Treatment**: Null values for batters are replaced with average values. In cases where certain statistics such as bowling strike rates are not available, external data from Google is used to fill in the gaps.

## Methodology

1. **Data Cleaning**: Removal of uncapped players and players with less than 10 matches.
2. **Data Imputation**: Filling null values with averages or externally sourced data.
3. **Analysis**: Identifying top performers based on key performance indicators relevant to batters and all-rounders.

## Tools Used

- Data analysis and cleaning: Python (Pandas)
- Visualization: Matplotlib, Seaborn
- Data sourcing: Google (for missing data points)

## Results
Look for the TOP 5 Batsman,bowler, all rounder for buying players.
## How to Navigate This Repository

- **data/**: Contains the raw and cleaned datasets.
- **notebooks/**: Jupyter notebooks with the analysis code and findings.
- **scripts/**: Python scripts used for data cleaning and analysis.
- **visualizations/**: Charts and graphs generated from the analysis.
