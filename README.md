# Graph VPint

### Urban Computing 2026-2027, Group 4: Sotiris Gypsiotis, Sude Şahin.
--------------------------------------------------

Extending VPint ([Arp et al., 2022](https://link.springer.com/article/10.1007/s10618-022-00843-2)) from grids to graphs, so it can interpolate missing values at irregular point locations directly instead of gridding the data first.

## Data

We use the UK Department for Transport road traffic counts for the London region. See [`data/README.md`](data/README.md) for what to download and where to put it, and [`notebooks/01_data_exploration.ipynb`](notebooks/01_data_exploration.ipynb) for why we chose London.

## Setup

Python 3.11 (the original VPint code needs `numpy` 1.26, which does not support Python 3.13+).

```bash
python -m venv .venv
source .venv/bin/activate # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

`requirements.txt` installs the original [VPint code](https://github.com/ADA-research/VPint) as a dependency, pinned to the paper version.

## Layout

| Folder | Contents |
|---|---|
| `data/` | Downloaded CSVs (not committed) and a README on where to get them |
| `notebooks/` | Data exploration |
| `graph_vpint/` | Our method: graph construction, propagation, weights |
| `baselines/` | IDW, kriging, original grid VPint |
| `experiments/` | Experiment scripts |

## Licence

GPL-3.0, because we build on the GPL-3.0 VPint code. The DfT data is under the Open Government Licence v3.0.
