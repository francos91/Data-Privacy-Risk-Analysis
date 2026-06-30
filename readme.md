# Data Science Portfolio: Privacy & Risk Analysis

**Author:** Franco Saayman | Stellenbosch University  
**Project:** Post-block Assignment 1 — Task A & Task B

---

## 📋 Overview
This project performs an automated privacy assessment and mitigation analysis on the `Amazon_Reviews` dataset. It is divided into two modules:
* **Task A:** Threat Assessment (Re-identification risks, linkage attacks, and entropy analysis).
* **Task B:** Mitigation & ROI (Generalisation, Suppression, Differential Privacy, and financial risk modeling).

---

## 🛠 Prerequisites

### Environment
* **Python:** 3.8 or higher.
* **Dependencies:** `pandas`, `numpy`, `scipy`, `matplotlib`, `seaborn`.

### Installation
Run the following command in your terminal to install all required libraries:

```bash
pip install pandas numpy scipy matplotlib seaborn
Note: No machine learning libraries (e.g., scikit-learn) are required for this project.

📂 File Structure
Ensure your directory is organized as follows before execution:

Plaintext
project_root/
├── Amazon_Reviews.csv    # Source dataset
├── task_a.py             # Threat Assessment logic
└── task_b.py             # Mitigation & ROI logic
🚀 Execution
Open your terminal or command prompt in the project directory and execute the scripts:

Task A (Threat Assessment)
Bash
python task_a.py
Task B (Mitigation & ROI)
Bash
python task_b.py
(If python is not recognized, try python3 instead.)

📊 Expected Output
Task A
Duration: ~10–20 seconds.

Output: Creates task_a_outputs/ with subfolders for /figures and /results.

Task B
Duration: ~1–2 minutes.

Output: Creates task_b_outputs/ with subfolders for /figures and /results.

 Troubleshooting
Problem	Solution
ModuleNotFoundError	Run pip install pandas numpy scipy matplotlib seaborn
FileNotFoundError	Ensure Amazon_Reviews.csv is in the same folder as the script.
Figure quality/overlap	Run pip install --upgrade matplotlib
Permission denied	Run terminal as Administrator or use python -m pip install ...
 System Requirements
OS: Windows 10/11, macOS 10.14+, or Linux (Ubuntu 20.04+).

RAM: 4 GB minimum.

Disk Space: ~50 MB for generated outputs.


***

### Instructions for GitHub:
1. Go to your repository on GitHub.
2. Click **"Add file"** > **"Create new file"**.
3. Name the file `README.md`.
4. Paste the content above directly into the edit box.
5. Scroll down and click **"Commit changes"**.
