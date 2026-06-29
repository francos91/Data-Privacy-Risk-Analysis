
README — How to Execute the Code for Task A and Task B in Python
Data Science Portfolio Project | Post-block Assignment 1
Author: Franco Saayman | Stellenbosch University
PREREQUISITES
================================================================================

Software required:

Python 3.8 or higher

pip (Python package manager)

Python libraries required:

pandas

numpy

scipy

matplotlib

seaborn

Install all dependencies with one command:

pip install pandas numpy scipy matplotlib seaborn
NB: No external libraries like faker, reportlab, or scikit-learn are required.
No machine learning model training is performed.

FILE STRUCTURE (before running)
================================================================================

Place these files in the SAME folder:

your_folder/
├── Amazon_Reviews.csv                  ← the dataset
├── task_a.py                           ← Task A code (Threat Assessment)
├── task_b.py                           ← Task B code (Mitigation & ROI)
└── README.txt                          ← this file
HOW TO RUN THE TASKS
================================================================================

Open a terminal/command prompt, navigate to the folder, and run:

For Task A:
python task_a.py

For Task B:
python task_b.py

On some systems, you may need to use:
python3 task_a.py
python3 task_b.py

WHAT TO EXPECT WHEN RUNNING
================================================================================

TASK A:
When you run the script, it will print progress to the console [1/6] to [6/6].
It will take approximately 10–20 seconds to run completely.
It will automatically create a folder named task_a_outputs in the same directory.
Inside task_a_outputs, it will create two subfolders: figures and results.

TASK B:
When you run the script, it will print progress detailing Generalisation,
Suppression, Differential Privacy, and ROI calculations.
It will take approximately 1-2 minutes to run completely.
It will automatically create a folder named task_b_outputs in the same directory.
Inside task_b_outputs, it will create two subfolders: figures and results.

OUTPUT FILES GENERATED
================================================================================

task_a_outputs/
├── figures/
│   ├── figure1_eda_overview.png            ← 2x2 EDA dashboard
│   ├── figure2_reidentification_risk.png   ← Uniqueness & K-anonymity charts
│   ├── figure3_linkage_attack.png          ← Simulated attack results
│   ├── figure4_crisp_dm_trajectory.png     ← Modified CRISP-DM diagram
│   └── figure5_entropy_heatmap.png         ← Joint entropy matrix
│
└── results/
├── qi_uniqueness_results.csv           ← All 63 QI combination results
├── linkage_attack_results.csv          ← Attack success rates per scenario
└── synthetic_reviews.csv               ← Generated synthetic review data

task_b_outputs/
├── figures/
│   ├── figure6_generalisation.png          ← Generalisation reduction
│   ├── figure7_suppression.png             ← k-Anonymity retention vs quality
│   ├── figure8_differential_privacy.png    ← DP error vs epsilon
│   ├── figure9_before_after.png            ← Privacy improvement comparison
│   └── figure10_roi.png                    ← ZAR ROI Value Bridge
│
└── results/
├── generalisation_results.csv          ← Mitigation outputs
├── suppression_results.csv

├── differential_privacy_results.csv

├── roi_analysis.csv                    ← POPIA financial risk values
└── combined_recommendation.csv         ← Final business case

TROUBLESHOOTING
================================================================================

Problem: "ModuleNotFoundError: No module named 'pandas'"
Solution: Run  pip install pandas numpy scipy matplotlib seaborn

Problem: "ERROR: Cannot find 'Amazon_Reviews.csv'"
Solution: Make sure Amazon_Reviews.csv is in the SAME folder as the .py file.
Do not rename the CSV file.

Problem: Script runs but figures look wrong or text overlaps
Solution: Ensure matplotlib version is 3.5+ by running:
pip install --upgrade matplotlib

Problem: "python" command not found
Solution: Try "python3" instead, or check your Python installation.

Problem: Permission error on Windows
Solution: Run the terminal as Administrator, or use:
python -m pip install pandas numpy scipy matplotlib seaborn

SYSTEM REQUIREMENTS
================================================================================

Operating System:  Windows 10/11, macOS 10.14+, or Linux (Ubuntu 20.04+)
Python:            3.8 or higher
RAM:               4 GB minimum
Disk Space:        ~50 MB for all outputs

================================================================================
END OF README
