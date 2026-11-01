# Data

The CSV files are not committed (see `.gitignore`). Download them yourself and place them in this folder.

| File | What it is | Download |
|---|---|---|
| `dft_traffic_counts_aadf.csv` | Annual average daily flow (vehicles per day) per count point per year, 2000–2025, with coordinates, road category and whether the value was counted or estimated | [DfT downloads](https://roadtraffic.dft.gov.uk/downloads), row "Annual average daily flow", CSV |
| `count_points.csv` | One row per count point: location and road details | Same page, row "Count points", CSV |

The file names don't need to match exactly. The notebook looks for any CSV with `aadf` in its name (excluding the by-direction file) and any CSV with `count_point` in its name.

Column definitions: [DfT metadata document](https://storage.googleapis.com/dft-statistics/road-traffic/all-traffic-data-metadata.pdf).

Source: Department for Transport, road traffic statistics. Published under the [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).
