# BT4222 Project: Strategic Lifecycle Recommendation Architecture (SLRA) for Anime
This repository contains the source code and datasets for our BT4222 project. Our study focuses on implementing a Hybrid Recommendation Architecture to solve the Cold Start problem for new users while surfacing niche content for enthusiasts. Using the MyAnimeList dataset, we developed and compared multiple models, including Matrix Factorization, Neural Matrix Factorization and Deep Learning-based architectures.

## Datasets
**Raw Data:** https://www.kaggle.com/datasets/dbdmobile/myanimelist-dataset

**Processed Data**: https://drive.google.com/drive/folders/15nXaToCyI_qNokhzCH65sI5vlsB1hfEd

## Google Colab Setup & File Requirements
| Step | Notebook Name | Input Files Required | Output Files Generated |
| :--- | :--- | :--- | :--- |
| 1 | `step1_data_cleaning.ipynb` | `anime-filtered.csv.zip`, `user_filtered.csv.zip`, `users-details-2023.csv.zip` | `anime_clean.csv`, `users_clean.csv`, `ratings_clean.csv`  |
| 2 | `step2_data_exploration_and_preparation.ipynb` | `anime_clean.csv`, `users_clean.csv`, `ratings_clean.csv` | `users_sampled.csv`, `ratings_sampled.csv` |
| 3 | `step3_feature_engineering.ipynb` | `anime_clean.csv`, `users_sampled.csv`, `ratings_sampled.csv` | `users_sampled_engineered.csv`, `ratings_sampled_engineered.csv` |
| 4 | `step4_matrix_factorization.ipynb` | `anime_clean.csv`, `users_sampled_engineered.csv`, `ratings_sampled_engineered.csv` | |
| 5 | `step5_neural_matrix_factorization.ipynb` | `anime_clean.csv`, `users_sampled_engineered.csv`, `ratings_sampled_engineered.csv`| |
| 6 | `step6_evaluation_of_mf_nmf.ipynb` | `anime_clean.csv`, `users_sampled_engineered.csv`, `ratings_sampled_engineered.csv`| |
| 7a | `step7a_two_tower_metadata.ipynb` | `anime_10pct.csv`, `users_10pct.csv`, `ratings_10pct.csv` | |
| 7b | `step7b_two_tower_reviews.ipynb` | `anime_clean.csv`, `jikan_crawled_reviews_with_userid.csv` | |


**How to Run on Colab?**
1. Open the desired .ipynb file in Google Colab.
2. Click on the **Files** icon on the left panel and select "Upload to session storage". Upload the required input files listed in the table above.
3. Run all cells.

**Note:** Each notebook is standalone. Intermediary data from previous steps has been provided as separate inputs to ensure each script runs without dependencies.
