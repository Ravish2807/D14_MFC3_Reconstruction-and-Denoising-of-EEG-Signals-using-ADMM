<p align="center">
  <img src="logo.svg" alt="Project Logo" width="300">
</p>

<div align="center">

# $$\huge \color{#007ACC}{\text{Mathematics for Computing 3}}$$

## $$\Large \color{#D9730D}{\mathbf{Reconstruction\ and\ Denoising\ of\ the\ EEG\ signals\ using\ ADMM}}$$

![Tech](https://img.shields.io/badge/Tools-Python%20|%20MATLAB%20|%20LaTeX-blueviolet?style=for-the-badge)

</div>

<p align="center">
  Presented by: <b>Group-14, AIE-D</b>
</p>

---
  
### 👥 Team Members
| Name | Roll Number |
| :--- | :--- |
| <img src="https://img.shields.io/badge/Ravishanmugam%20K-blue?style=flat-square" /> | `CB.SC.U4AIE24347` |
| <img src="https://img.shields.io/badge/Sharvesh%20Sivaganam-blue?style=flat-square" /> | `CB.SC.U4AIE24355` |
| <img src="https://img.shields.io/badge/Sri%20Harini%20MP-blue?style=flat-square" /> | `CB.SC.U4AIE24358` |
| <img src="https://img.shields.io/badge/Vignes%20VM-blue?style=flat-square" /> | `CB.SC.U4AIE24359` |

---

> [!IMPORTANT]
> **Project Overview:** This project focuses on the reconstruction and denoising of EEG signals using the **Alternating Direction Method of Multipliers (ADMM)**. The zip file contains the Jupyter Notebook, MATLAB LiveScript, and the final presentation.

> [!NOTE]
> **Base Paper:** *"Reconstruction and Denoising of EEG Signal Using Alternating Direction Method of Multipliers"* (included as `Reconstruction_and_Denoising_of_EEG_Signal_Using_Alternating_Direction_Method_of_Multipliers.pdf`)

---

## 📌 About the Project

This project focuses on the **reconstruction and denoising of Electroencephalogram (EEG) signals** using the **Alternating Direction Method of Multipliers (ADMM)**.

EEG signals are highly sensitive and often corrupted by noise such as eye blinks, muscle activity, and external interference. To address this, the project applies **ADMM-based optimization**, which efficiently solves complex problems by breaking them into smaller subproblems.

- EEG reconstruction is performed using an **ℓ₁-regularized framework** to promote sparsity.
- Denoising is achieved using a **Lasso-based ADMM approach** under:
  - Gaussian noise  
  - Laplacian noise  
- **Independent Component Analysis (ICA)** is used to remove artifacts like eye and muscle noise.
- The dataset is taken from **PhysioNet**, consisting of 36 subjects performing mental arithmetic tasks.

The project evaluates performance using **RMSE**, along with time-domain and frequency-domain analysis, demonstrating effective reconstruction and noise removal.

---

### 📊 Dataset Details
* **Data Source:** [PhysioNet EEG Arithmetic Dataset](https://physionet.org/content/eegmat/1.0.0/)
* **Description:** Signal readings from 36 subjects covering **Case-1** (Before math task) and **Case-2** (After math task).
* **Software:** Preferred viewer for 23-channel reading: **Polyman**.

---

### 📁 File Descriptions & Use Cases

| File Path | Description |
| :--- | :--- |
| <code style="color: green">Batch_EEG_Processing.ipynb</code> | **Full dataset automation.** Reads EDF, maps metadata, runs ADMM. |
| `Jounral_Paper_D14_MFC3/` | Journal Paper files in LaTeX. |
| `Journal_Paper_D14_MFC3/D14_MFC3_Paper.pdf` | Draft Paper for the obtained results. |
| `Journal_Paper_D14_MFC3/D14_MFC3_Paper.synctex.gz` | SyncTeX File for main LaTeX File. |
| `Journal_Paper_D14_MFC3/D14_MFC3_Paper.tex` | Main LaTex File for the Paper. |
| `Journal_Paper_D14_MFC3/fig$_cell$$.png` | Images for results selected from the results folder. |
| `results/` | Results in terms of Time and Frequency Domain Plots. |
| `results/Reconstruction/` | Original vs Reconstructed time-domain plot PNGs. |
| `results/Denoised/` | Original vs Denoised time-domain plot PNGs. |
| `results/Frequency/` | Frequency-domain plots (Original, Noisy, Denoised). |
| `results/results_summary.csv` | Per-subject **RMSE** values. |
| `results/summary_stats.csv` | Group/task wise aggregate RMSE stats. |
| `results/comparison_plot.png` | Bar plot comparisons between groups/tasks. |
| `D14_MFC3_Paper.pdf` | Initial Journal Paper Draft. |
| `Final_Review.pptx` | Presentation for the project update. |
| `Reconstruction&Denoising_ADMM.ipynb` | Jupyter Lab documentation file. |
| `Reconstruction&Denoising_ADMM.mlx` | MATLAB LiveScript documentation file. |
| `Reconstruction&Denoising_ADMM.pdf` | PDF version of the MATLAB documentation. |
| `channel.png` | Visualization of the 23-channel systems. |
| `eeg-signal1.jpg` | Rough curve visualization and channel locations. |
| `soft.png` | Soft-Thresholding function visualization. |

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
├── eeg-during-mental-arithmetic-tasks-1.0.0/  (Dataset)
│   ├── subject-info.csv
│   ├── Subject01_1.edf
│   ├── Subject01_2.edf
│   ├── ...
│   └── Subject36_2.edf
├── Journal_Paper_D14_MFC3/                    (Draft Paper) 
|   ├──D14_MFC3_Paper.pdf
|   ├──D14_MFC3_Paper.synctex.gz
|   ├──D14_MFC3_Paper.tex
|   ├──fig1_cell12.png
|   ├──fig2_cell28.png
|   ├──fig3_cell30.png
|   ├──fig4_cell39.png
|   ├──fig5_cell40.png
|   ├──fig6_cell45.png
└── results/                                        
    ├── results_summary.csv
    ├── summary_stats.csv
    ├── comparison_plot.png
    ├── Reconstruction/
    │   ├── Subject01_1_reconstruction.png
    │   ├── Subject01_2_reconstruction.png
    │   └── ...
    ├── Denoised/
    │   ├── Subject01_1_denoising.png
    │   ├── Subject01_2_denoising.png
    │   └── ...
    └── Frequency/
        ├── Subject01_1_freq_original.png
        ├── Subject01_1_freq_noised.png
        ├── Subject01_1_freq_denoised.png
        ├── Subject01_2_freq_original.png
        └── ...
```
---
## 📚 References

1. *Reconstruction and Denoising of EEG Signal Using Alternating Direction Method of Multipliers*, Base Paper

2. Boyd, S., Parikh, N., Chu, E., Peleato, B., & Eckstein, J. (2011).  
   *Distributed Optimization and Statistical Learning via the Alternating Direction Method of Multipliers*.  

3. Donoho, D. L. (2006).  
   *Compressed Sensing*. IEEE Transactions on Information Theory.  

4. Candès, E. J., Romberg, J., & Tao, T. (2006).  
   *Robust Signal Recovery from Incomplete Data*.  

5. Tibshirani, R. (1996).  
   *Regression Shrinkage and Selection via the Lasso*.  

6. Hyvärinen, A., & Oja, E. (2000).  
   *Independent Component Analysis: Algorithms and Applications*.  

7. Rudin, L. I., Osher, S., & Fatemi, E. (1992).  
   *Nonlinear Total Variation Based Noise Removal Algorithms*.  

8. Goldberger, A. L., et al. (2000).  
   *PhysioBank, PhysioToolkit, and PhysioNet*.  

9. PhysioNet Dataset:  
   https://physionet.org/content/eegmat/1.0.0/
---
