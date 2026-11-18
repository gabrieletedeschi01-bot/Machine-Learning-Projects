# Car Racing — Image Classification

## Objective

Train convolutional neural networks to classify images from a 2D car-racing environment into five driving actions:

| Label | Action |
|---|---|
| 0 | Do nothing |
| 1 | Steer left |
| 2 | Steer right |
| 3 | Gas |
| 4 | Brake |

## Approach

The coursework implementation includes:
- A baseline CNN and a deeper CNN.
- Hyperparameter tuning for learning rate, batch size, convolutional architecture and fully connected layers.
- Evaluation using accuracy, weighted precision, recall and F1-score, classification report, confusion matrix, and training/validation curves.

Images are processed at 96×96 RGB resolution and normalized before training. Refer to the report for the detailed experimental setup and results.

## Contents

- `homework_2.py` — data loading, model training, tuning and evaluation.
- `report/report.pdf` — coursework report.

## Dataset

The supplied image dataset is intentionally not included in this repository. Obtain the original dataset from the course materials and extract it locally so that the following structure is available:

```text
data/
└── public/
    ├── train/
    │   ├── 0/
    │   ├── 1/
    │   ├── 2/
    │   ├── 3/
    │   └── 4/
    └── test/
        ├── 0/
        ├── 1/
        ├── 2/
        ├── 3/
        └── 4/
```

The script expects the images under `data/public/`.

## Run

Install the required packages, then run from this project directory:

```bash
pip install numpy tensorflow scikit-learn pillow matplotlib seaborn
python homework_2.py
```

Training and hyperparameter tuning can be computationally intensive; a GPU is recommended.
