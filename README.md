# Defect Quality System

An anomaly detection workflow for the MVTec AD dataset using PatchCore and `anomalib`. The notebook trains and evaluates a separate model for each category in `datasets/`, then stores the outputs under `results/`.

## Results

The current run produced consistently strong performance across the dataset. Notable highlights include:

- `bottle`: image AUROC `1.0000`, pixel AUROC `0.9784`
- `hazelnut`: image AUROC `0.9989`, pixel AUROC `0.9892`
- `leather`: image AUROC `0.9969`, pixel AUROC `0.9893`
- `metal_nut`: image AUROC `0.9951`, pixel AUROC `0.9835`
- `screw`: image AUROC `0.9528`, pixel AUROC `0.9917`

Across the 15 categories, image AUROC stays high overall, showing that PatchCore is a strong fit for this defect detection task.

## Dataset License

This project uses the MVTec AD dataset. The dataset license is Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International, so it is intended for non-commercial use.

See `datasets/license.txt` for the full license text.