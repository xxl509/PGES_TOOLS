PGES Detection Tool
  This repository contains the code for the Postictal Generalized EEG Suppression (PGES) detection tool. Due to the large size of the pipeline file and training data, these files cannot be uploaded to GitHub. Please contact the author for access to these files.

Prerequisites
  To utilize the PGES detection tool, please ensure you have the following:


Setup Instructions
  1. Download Files: Contact the author to obtain the pipeline and training_data.npy files.
  2. Directory Structure: Ensure that the pipeline folder and training_data.npy are located in the same directory.
  3. File Naming Convention: Maintain the specified naming convention for your signal CSV files, e.g., 001_post_ictal_eeg_1024Hz.csv.

Usage
  To execute the PGES detection tool, follow these steps:
  1. Open a terminal or command prompt.
  2. Navigate to the directory containing the pipeline folder and your signal data CSV file.
  3. Run the following command:
    bash
    Copy code
    ./pipeline /the/path/of/your/signal_data.csv

Output
  Upon execution, a result folder will be generated. Inside this folder, you will find a .npy file containing probabilities for each second of the provided signal data. These probabilities indicate the likelihood of the end of PGES, with higher values signifying a greater likelihood.

Contact
  For any questions or requests for additional files, please contact the authors of this paper: https://www.frontiersin.org/journals/neuroinformatics/articles/10.3389/fninf.2022.1040084/full.

Thank you!
