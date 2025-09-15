# Qatar 2022 Goals Prediction

A reproducible repository for a goal prediction model using events data (Qatar 2022).

## Quickstart
```bash
conda env create -f environment.yml
conda activate qatar2022
python -m src.qatar_goals.train --data data/raw/events.csv --model-out models/baseline.joblib
