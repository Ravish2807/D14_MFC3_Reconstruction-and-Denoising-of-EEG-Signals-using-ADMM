                                  Mathematics for Computing 3 , Project Folder ReadMe File


Presented by 
Group-14 ,AIE-D

Team members:
Ravishanmugam K       -- CB.SC.U4AIE24347 ​
Sharvesh Sivaganam    -- CB.SC.U4AIE24355​
Sri Harini MP         -- CB.SC.U4AIE24358​
Vignes VM             -- CB.SC.U4AIE24359




Our Project title: "Reconstruction and Denoising of the EEG signals using ADMM"

The zip file contains the juypter notebook file , matlab livescript file with the pdf version of our project and our Final presentation.Some images also contained in the Zip file , which is used in the JupyterLab Notebook documentation Purpose.
Our base paper is "Reconstruction_and_Denoising_of_EEG_Signal_Using_Alternating_Direction_Method_of_Multipliers.pdf"

As the dataset size > 10MB , further details about that is mentioned below.

As the data used in the project is an signal , to view the signal , an external software is used to view the signal of an subject with the 23 channel reading.The software preferred by the Data source is "Polyman" for reading the eeg signals , which is available for windows , Linux and Mac. There are totally 36 subjects means 36 humans were performed the eeg signal test for some 2.5 minutes with two cases , case-1:before arithemetic task and case-2: after math task to monitor more in depth about the human brain activity during the stress in work. The test performed before math task is named as "subjectxx_0.edf" , where after the math task performed eeg is named as "subjectxx_1.edf".

Further details about the data in in the link  "https://physionet.org/content/eegmat/1.0.0/".

The images "channel1.jpg" shows the placement of the 23 channels in the human brain , which is used in the juypter documentation.

"eeg-signal1.jpg" show the rough curve how it will look like , the original signal reading is attached in the ppt.
"soft.jpg" shows the impact of an curve under an mathematical operation named soft threshold , which will be used to explain in the juypter lab documentation.

The pdf file named "Reconstruction_and_Denoising_of_EEG_Signal_Using_Alternating_Direction_Method_of_Multipliers.pdf", is the base paper for this project.

Batch processing Python notebook for full dataset automation is named as "Batch_EEG_Processing.ipynb" and performs the following:
- Reads all EDF files under the dataset path (before and during task: subject##_1.edf and subject##_2.edf)
- Loads subject metadata from "subject-info.csv" and maps group labels (G / B)
- Runs each file through ADMM reconstruction, noise injection, ADMM denoising, and frequency spectrum analysis
- Saves per-subject output plots in organized folders

Project root path:
- c:\AIE Files\Projects\S3\D_14

Auto-generated results folder hierarchy (under project root):
- results\ : base results folder
- results\Reconstruction\ : original vs reconstructed time-domain plot PNGs
- results\Denoised\ : original vs denoised time-domain plot PNGs
- results\Frequency\ : frequency-domain plot PNGs for original, noisy, denoised signals
- results\results_summary.csv : per-subject RMSE values
- results\summary_stats.csv : group/task aggregate RMSE stats in scientific notation
- results\comparison_plot.png : bar plot comparisons between groups/tasks

File Present and their use case in the Project is described as , 

Juypter lab documentation file is named as                                        "Reconstruction&Denoising_ADMM.ipynb"
MATLAB livescript documentation file is named as                                  "Reconstruction&Denoising_ADMM.mlx"
Presentation for the update of the project is named as                            "Final_Review.pptx".
The pdf version of the matlab ddocumentation is named as                          "Reconstruction&Denoising_ADMM.pdf"
The 23 channel systems of the EEG signal is described in the image named as       "channel.png"
The EEG signal and the location of the channel is described in the image named as "eeg-signal1.jpg"
Soft-Thresholding function related to the ADMM is described in the image named as "soft.png"  
Reconstruction and Denoising for all the subjects has computed and named as       "Batch_EEG_Processing.ipynb"


 





Thank You


