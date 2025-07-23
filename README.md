# RFCDE model for fuzzy clustering
This repository provides the MATLAB implementation of our method RFCDE, proposed in the paper "Outlier Resistant Fuzzy Clustering via Row Sparse Discriminative Embedding Projection."
The paper is currently under review. The full code and documentation will be released upon acceptance.
RFCDE consists of four main stages:
1.	Estimating sample contributions to adaptively identify outliers;
2.	Refining fuzzy memberships using a row-sparse outlier-aware constraint;
3.	Learning cluster prototypes in projection space;
4.	Optimizing a discriminative embedding that maximizes inter-class separability while minimizing reconstruction error.

# Repository Structure
•	Initialize/ – Different initialization strategies for the clustering algorithm.

•	Results_ave/ – Stores the averaged results from repeated experiments on benchmark datasets.

•	funs/ – Common utility functions used in the algorithm.

•	Dataset/ – Contains benchmark datasets used for evaluation.

<img width="320" height="289" alt="image" src="https://github.com/user-attachments/assets/565fcb0c-67d8-4372-82d5-5de83b5bb1ca" />

 
# Quantitative Evaluation
First, set the number of runs (e.g., nRuns = 10) and Choose the dataset(s) to test in Run_HISSM.m
Then, run Run_HISSM.m. All results in the paper are obtained through repeated experiments under the same settings and are saved automatically.

# Results Format
Each independent run outputs the following evaluation metrics:
•	Accuracy (ACC)
•	Normalized Mutual Information (NMI)
•	Purity (Pu)
•	Average Value (AVE.) across all runs
•	Standard Deviation (Std.)
For the results Results_AVE and Results_AVE_y under different initializations, Assuming the number of repetitions is set to 10, the results are logged and summarized in Results_ave/ as illustrated in the figure.

<img width="1965" height="382" alt="image" src="https://github.com/user-attachments/assets/2f6c62f2-0ade-4be2-8643-1d247bae70af" />
<img width="1964" height="382" alt="image" src="https://github.com/user-attachments/assets/e156e37f-1740-40c5-96eb-f391f859c524" />


