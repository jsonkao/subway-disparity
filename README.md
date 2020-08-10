## Setup

1. Run `make`. This pulls Chris Whong's [turnstile data](https://qri.cloud/nyc-transit-data/turnstile_daily_counts_2020) and runs a point-to-polygon join to identify each station's census tract. The output file is `turnstile_data.csv`, which has columns `date`, `entries`, `exits`, and `GEOID`.

2. `report.Rmd` merges this file with [ACS data](https://www.census.gov/programs-surveys/acs), and then makes a  visualization.