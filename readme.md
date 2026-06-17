================================================================================
README — How to Execute the Code for Task A in Python
================================================================================
Data Science Portfolio Project | Post-block Assignment 1
Author: Franco Saayman | Stellenbosch University
================================================================================

1. PREREQUISITES
================================================================================

Software required:
  - Python 3.8 or higher
  - pip (Python package manager)

Python libraries required:
  - pandas
  - numpy
  - scipy
  - matplotlib
  - seaborn

Install all dependencies with one command:

    pip install pandas numpy scipy matplotlib seaborn


NB: No external libraries like faker, reportlab, or scikit-learn are required.
      No machine learning model training is performed.


2. FILE STRUCTURE (before running)
================================================================================

Place these files in the SAME folder:

    your_folder/
    ├── Amazon_Reviews.csv                  ← the dataset
    ├── task_a.py                           ← Task A code
    └── README.txt                          ← this file



3. HOW TO RUN TASK A
================================================================================

Open a terminal/command prompt, navigate to the folder, and run:

    cd your_folder
    python task_a.py

On some systems, you may need to use:
    python3 task_a.py


4. WHAT TO EXPECT WHEN RUNNING
================================================================================

When you run the script, it will print progress to the console [1/6] to [6/6].
It will take approximately 10–20 seconds to run completely.

It will automatically create a folder named `task_a_outputs` in the same directory.
Inside `task_a_outputs`, it will create two subfolders: `figures` and `results`.


5. OUTPUT FILES GENERATED
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


6. TROUBLESHOOTING
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


7. SYSTEM REQUIREMENTS
================================================================================

  Operating System:  Windows 10/11, macOS 10.14+, or Linux (Ubuntu 20.04+)
  Python:            3.8 or higher
  RAM:               4 GB minimum
  Disk Space:        ~50 MB for all outputs


================================================================================
END OF README
================================================================================