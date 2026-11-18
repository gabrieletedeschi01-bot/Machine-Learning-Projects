# Machine Learning Projects

Two coursework projects completed for the **Machine Learning** course (A.Y. 2024/2025).

## Projects

### 1. Robot Forward Kinematics — Regression
[`homework-1-robot-kinematics/`](homework-1-robot-kinematics/)

Regression models learn the forward kinematics of planar and spatial robot manipulators, mapping joint configurations to end-effector positions. The coursework explores 2R, 3R and 5R manipulators, model selection, evaluation across datasets generated with different random seeds, and Jacobian estimation/comparison where covered in the report.

### 2. Car Racing — Image Classification
[`homework-2-car-racing/`](homework-2-car-racing/)

Convolutional neural networks classify images from a 2D car-racing environment into five driving actions: do nothing, steer left, steer right, gas and brake. The experiments compare CNN architectures and tune hyperparameters, with evaluation using accuracy, weighted precision/recall/F1, a classification report and a confusion matrix.

## Repository structure

```text
.
├── README.md
├── .gitignore
├── homework-1-robot-kinematics/
│   ├── README.md
│   ├── homework_1.py
│   └── Homework_1_Machine_Learning.pdf
│   
└── homework-2-car-racing/
    ├── README.md
    ├── homework_2.py
    └── Homework_2_Machine_Learning.pdf
```

## Datasets

The original CSV and image datasets are intentionally **not tracked** in this repository to keep it lightweight. The scripts expect the original datasets in the locations described in each project's README. They must be obtained separately from the original course materials and placed in the expected folders before running the experiments.

## Notes

These are academic coursework implementations. Refer to the individual reports for the experimental setup and results. The scripts may require adjustment for different local environments or library versions.
