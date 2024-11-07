A hybrid unsupervised and supervised learning approach for postictal generalized EEG suppression detection

Sudden unexpected death of epilepsy (SUDEP) is a catastrophic and fatal complication of epilepsy and is the primary cause of mortality in those who have uncontrolled seizures. While several multifactorial processes have been implicated including cardiac, respiratory, autonomic dysfunction leading to arrhythmia, hypoxia, and cessation of cerebral and brainstem function, the mechanisms underlying SUDEP are not completely understood. Postictal generalized electroencephalogram (EEG) suppression (PGES) is a potential risk marker for SUDEP, as studies have shown that prolonged PGES was significantly associated with a higher risk of SUDEP. Automated PGES detection techniques have been developed to efficiently obtain PGES durations for SUDEP risk assessment. However, real-world data recorded in epilepsy monitoring units (EMUs) may contain high-amplitude signals due to physiological artifacts, such as breathing, muscle, and movement artifacts, making it difficult to determine the end of PGES. In this paper, we present a hybrid approach that combines the benefits of unsupervised and supervised learning for PGES detection using multi-channel EEG recordings. A K-means clustering model is leveraged to group EEG recordings with similar artifact features. We introduce a new learning strategy for training a set of random forest (RF) models based on clustering results to improve PGES detection performance. Our approach achieved a 5-second tolerance-based detection accuracy of 64.92%, a 10-second tolerance-based detection accuracy of 79.85%, and an average predicted time distance of 8.26 seconds with 286 EEG recordings using leave-one-out (LOO) cross-validation. The results demonstrated that our hybrid approach provided better performance compared to other existing approaches.

PGES Detection Tool
  This repository contains the code for the Postictal Generalized EEG Suppression (PGES) detection tool. Due to the large size of training data, these files cannot be uploaded to GitHub. Please contact the author for additional access.

Prerequisites
  To utilize the PGES detection tool, please ensure you have the following:


Setup Instructions
  1. Ensure "pipeline.pyc" and "training_data.npy" are located in the same directory.
  2. Install conda.
  3. Establish a conda environment by executing the command "conda env create -f environment.yml".
  4. File Naming Convention: Maintain the specified naming convention for your signal CSV files, e.g., 001_post_ictal_eeg_1024Hz.csv.
  5. Activate the conda environment.

Usage
  To execute the PGES detection tool, follow these steps:
  1. Open a terminal or command prompt.
  2. Navigate to the directory containing the pipeline folder and your signal data CSV file.
  3. Run the following command: python pipeline.pyc /the/path/of/your/signal_data.csv

Output
  Upon execution, a result folder will be generated. Inside this folder, you will find a .npy file containing probabilities for each second of the provided signal data. These probabilities indicate the likelihood of the end of PGES, with higher values signifying a greater likelihood.

Contact
  For any questions or requests for additional files, please contact the authors of this paper: https://www.frontiersin.org/journals/neuroinformatics/articles/10.3389/fninf.2022.1040084/full.

Cite Our Work
1. Li X, Huang Y, Lhatoo SD, Tao S, Vilella Bertran L, Zhang GQ, Cui L. A hybrid unsupervised and supervised learning approach for postictal generalized EEG suppression detection. Frontiers in Neuroinformatics. 2022 Dec 19;16:1040084. (https://www.frontiersin.org/journals/neuroinformatics/articles/10.3389/fninf.2022.1040084/full)
2. Li X, Tao S, Jamal-Omidi S, Huang Y, Lhatoo SD, Zhang GQ, Cui L. Detection of postictal generalized electroencephalogram suppression: random forest approach. JMIR Medical Informatics. 2020 Feb 14;8(2):e17061. (https://medinform.jmir.org/2020/2/e17061)


Thank you!
