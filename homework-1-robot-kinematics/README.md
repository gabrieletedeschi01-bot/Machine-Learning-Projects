# Robot Forward Kinematics — Regression

## Objective

Train regression models to approximate the forward kinematics of robot manipulators, mapping joint angles to end-effector positions.

## Experiments

The coursework investigates:
- **2R planar robot:** Random Forest and feed-forward neural network regression, including Jacobian estimation and comparison with the analytical Jacobian.
- **3R planar robot:** XGBoost and K-nearest-neighbours regression, with Jacobian-related analysis.
- **5R spatial robot:** K-nearest-neighbours and neural-network regression.

The experiments include train/test splits, model selection and evaluation on datasets generated with different random seeds. See the report for the detailed methodology and results.

## Contents

- `homework_1.py` — implementation of the experiments and evaluation.
- `report/report.pdf` — coursework report.

## Dataset

The six original CSV files are not included in this repository. Obtain them from the original course materials and place them in a local `data/` directory, preserving these filenames:

```text
data/
├── r2_1000_100k.csv
├── r2_2000_100k.csv
├── r3_1000_100k.csv
├── r3_2000_100k.csv
├── r5_1000_100k.csv
└── r5_2000_100k.csv
```

The script reads the CSV files from that directory.

## Run

Install the required Python packages in your environment, then run from this project directory:

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow xgboost joblib scipy
python homework_1.py
```

Training and hyperparameter search can be computationally intensive. Generated models and outputs are local artifacts and are not tracked by Git.
