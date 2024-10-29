To utilize the PGES detection tool, please follow these steps:
1. Ensure "pipeline" and "training_data.npy" are located in the same directory.
2. Please keep the name convention of the signal CSV file, e.g., "001_post_ictal_eeg_1024Hz.csv".
3. Execute the command "./pipeline /the/path/of/your/signal_data.csv" to generate the result folder. Within this folder, you'll find an npy file containing probabilities for each second, signifying the potential end of PGES, with higher probabilities indicating a greater likelihood of the end of PGES.