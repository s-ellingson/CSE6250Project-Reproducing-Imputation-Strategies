# CSE6250Project-Reproducing-Imputation-Strategies

DEPENDENCIES:
numpy, scikit-learn, pandas, matplotlib, seaborn, pickle, os, tqdm, sys

DIRECTORY STRUCTURE:
- NOTE: All file calls are done relatively, meaning that as long as the directory structure is followed, there should be no needed file path changes.
Local directory structure should be like the following:

- project_folder
   - code
      - original_preprocessing.ipynb (preprocesses MIMIC info)
      - original_experiment.ipynb (splits, imputes, and runs predictive analysis on processed MIMIC dataset)
      - analysis_groups.ipynb (displays metrics from MIMIC predictive analysis results)
      - synthetic.ipynb (creates synthetic dataset, imputes, and runs predictive simulation)
      - mimic_utils.py (functions and classes that mimic scripts use)
      - synthetic_utils.py (functions and classes that synthetic script uses)
   - data
      - unzipped MIMIC .csv files
   - results
      - these will be rewritten after original_experiment.ipynb has run.

DOWNLOAD INSTRUCTIONS:
- MIMIC III dataset is required for this code to run successfully. It will have to be downloaded separately from [here](https://physionet.org/content/mimiciii/1.4/).
- Clone repository and organize like the structure above.

RUN PROCEDURES
1. MIMIC
   1. Run original_preprocessing.ipynb, which will output two .csv files that original_experiment.ipynb will use.
   2. Run original_experiment.ipynb, which will output classification results.
   3. Run analysis_groups.ipynb, which will output MIMIC results. There will be errors on certain cells, so the complete process must be done MANUALLY.
2. SYNTHETIC
   1. Run synthetic.ipynb, which will output synthetic data results.
