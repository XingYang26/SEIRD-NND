[README.md](https://github.com/user-attachments/files/34111743/README.md)
# SEIRD-NND Reproduction Code

This repository contains the Python scripts and input datasets used to reproduce the tables, figures, and supplementary analyses in the SEIRD-NND manuscript.

## Files and directories

| File or directory | Purpose |
|---|---|
| `seird_nnd.py` | Core SEIRD-NND model, state estimation, and prediction functions. |
| `reproduce.py` | Unified command-line entry point for running individual tables, figures, and sensitivity analyses. |
| `engine/run_table1_synthetic.py` | Table 1(a–b): synthetic experiments, parameter recovery, and state reconstruction. |
| `engine/run_table1_pelt.py` | Table 1(c): regime detection and comparison with PELT. |
| `engine/format_table1.py` | Formats and exports Table 1 results. |
| `initial/run_table2.py` | Table 2 and Figure 2: Shanghai case-study estimation and outputs. |
| `initial/run_table3.py` | Table 3 and Figure 3: Guangdong case-study estimation and outputs. |
| `initial/shared_reduced_fit.py` | Shared reduced-model estimation routines for the case studies. |
| `initial/table3_data.py` | Guangdong data loading, initialization, and fitting utilities. |
| `initial/preprocess_table2.py` | Shanghai observation preprocessing, including the quarantine-stock series. |
| `initial/plot_figure2_figure3.py` | Creates Figures 2 and 3 from the corresponding case-study outputs. |
| `initial/helper_evaluation.py` | Forecast-origin selection and evaluation metrics. |
| `initial/helper_forecast_baselines.py` | Persistence and standard SEIRD forecasting baselines. |
| `initial/helper_no_regime.py` | Time-varying, no-regime model utilities. |
| `engine/run_table4_forecast.py` | Table 4: rolling-origin forecasts and benchmark comparisons. |
| `engine/verify_table4.py` | Checks and formats Table 4 forecasting results. |
| `engine/plot_figure4.py` | Figure 4: forecast MAE and MAPE by horizon. |
| `engine/run_table5_no_regime.py` | Table 5(a): regime-switching ablation. |
| `engine/run_table5_no_spatial.py` | Table 5(b): spatial-coupling ablation. |
| `engine/run_g2_uncertainty.py` | G2: parameter and effective reproduction-number uncertainty. |
| `engine/run_g3_scaling.py` | G3: population-scaling sensitivity. |
| `engine/run_g4_imputation.py` | G4: Shanghai data-imputation sensitivity. |
| `engine/run_g5_gaussian.py` | G5: Gaussian-innovation diagnostics and covariance sensitivity. |
| `engine/run_g6_network.py` | G6: migration-strength and network-topology sensitivity. |
| `engine/datasets/shanghai/` | Input datasets for the Shanghai analysis. |
| `engine/datasets/guangdong/` | Input datasets for the Guangdong analysis. |
| `requirements.txt` | Python package dependencies. |
| `outputs/` | Directory created during execution for generated tables, figures, and intermediate files. |

## Dependencies

- Python 3.10 or newer
- NumPy >= 1.24
- pandas >= 1.5
- SciPy >= 1.10
- Matplotlib >= 3.7

Install the required Python packages with:

```bash
python -m pip install -r requirements.txt
```
