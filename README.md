<p align="center">
  <img src="logo.svg" alt="Project Logo" width="300">
</p>  

# Mathematics for Computing 3
## Reconstruction and Denoising of the EEG signals using ADMM

**Presented by:** Group-14, AIE-D

### 👥 Team Members
* **Ravishanmugam K** — CB.SC.U4AIE24347
* **Sharvesh Sivaganam** — CB.SC.U4AIE24355
* **Sri Harini MP** — CB.SC.U4AIE24358
* **Vignes VM** — CB.SC.U4AIE24359

---

### 📝 Project Overview
The zip file contains the Jupyter Notebook file, MATLAB LiveScript file with the PDF version of our project, and our Final presentation. Some images are also contained in the zip file, which are used for JupyterLab Notebook documentation purposes.

**Base Paper:** *"Reconstruction and Denoising of EEG Signal Using Alternating Direction Method of Multipliers"* (included as `Reconstruction_and_Denoising_of_EEG_Signal_Using_Alternating_Direction_Method_of_Multipliers.pdf`)

### 📊 Dataset Details
As the dataset size is > 10MB, further details are mentioned below:
* **Data Source:** [PhysioNet EEG Arithmetic Dataset](https://physionet.org/content/eegmat/1.0.0/)
* **Description:** Signal readings from 36 subjects (2.5 minutes duration) covering two cases: 
  1. Case-1: Before arithmetic task (`subjectxx_0.edf`)
  2. Case-2: After math task (`subjectxx_1.edf`)
* **Software:** The preferred software to view the 23-channel reading is **Polyman** (Windows, Linux, Mac).

---

### 📁 File Descriptions & Use Cases

| File Path | Description |
| :--- | :--- |
| `Batch_EEG_Processing.ipynb` | Batch processing Python notebook for full dataset automation. Reads EDF files, maps metadata, runs ADMM reconstruction/denoising, and saves results. |
| `Jounral_Paper_D14_MFC3/` | Journal Paper files in LaTeX. |
| `Journal_Paper_D14_MFC3/D14_MFC3_Paper.pdf` | Draft Paper for the obtained results. |
| `Journal_Paper_D14_MFC3/D14_MFC3_Paper.synctex.gz` | SyncTeX File for main LaTeX File (PDF to Tex locating). |
| `Journal_Paper_D14_MFC3/D14_MFC3_Paper.tex` | Main LaTex File for the Paper. |
| `Journal_Paper_D14_MFC3/fig$_cell$$.png` | Images for results selected from the results folder. |
| `results/` | Results in terms of Time and Frequency Domain Plots. |
| `results/Reconstruction/` | Original vs Reconstructed time-domain plot PNGs. |
| `results/Denoised/` | Original vs Denoised time-domain plot PNGs. |
| `results/Frequency/` | Frequency-domain plot PNGs for original, noisy, and denoised signals. |
| `results/results_summary.csv` | Per-subject RMSE values for Reconstruction and Denoising. |
| `results/summary_stats.csv` | Group/task wise aggregate RMSE stats in scientific notation. |
| `results/comparison_plot.png` | Bar plot comparisons between groups/tasks over the mean for both cases. |
| `D14_MFC3_Paper.pdf` | Initial Journal Paper Draft for the Project. |
| `Final_Review.pptx` | Presentation for the project update. |
| `Reconstruction&Denoising_ADMM.ipynb` | Jupyter Lab documentation file. |
| `Reconstruction&Denoising_ADMM.mlx` | MATLAB LiveScript documentation file. |
| `Reconstruction&Denoising_ADMM.pdf` | PDF version of the MATLAB documentation. |
| `channel.png` | Describes the 23-channel systems of the EEG signal. |
| `eeg-signal1.jpg` | Rough curve visualization and channel locations. |
| `soft.png` | Soft-Thresholding function related to the ADMM. |

---

### 🌲 Project Tree Structure
```text
D14_MFC3_Reconstruction-and-Denoising-of-EEG-Signals-using-ADMM/
├── Batch_EEG_Processing.ipynb
├── Reconstruction&Denoising_ADMM.ipynb
├── Reconstruction&Denoising_ADMM.mlx
├── D14_MFC3_Paper.pdf
├── Reconstruction&Denoising_ADMM.pdf
├── Final_Review.pptx
├── ReadMe.txt
├── channel.png
├── eeg-signal1.jpg
├── soft.png
├── eeg-during-mental-arithmetic-tasks-1.0.0/
│   ├── subject-info.csv
│   ├── Subject01_1.edf
│   ├── Subject01_2.edf
│   ├── ...
│   └── Subject36_2.edf
├── Journal_Paper_D14_MFC3/
│   ├── D14_MFC3_Paper.pdf
│   ├── D14_MFC3_Paper.synctex.gz
│   ├── D14_MFC3_Paper.tex
│   ├── fig1_cell12.png
│   ├── fig2_cell28.png
│   ├── fig3_cell30.png
│   ├── fig4_cell39.png
│   ├── fig5_cell40.png
│   └── fig6_cell45.png
└── results/
    ├── results_summary.csv
    ├── summary_stats.csv
    ├── comparison_plot.png
    ├── Reconstruction/
    ├── Denoised/
    └── Frequency/
