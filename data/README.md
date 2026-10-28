# Dataset Information

This study utilizes the publicly available **OkCupid Profiles** dataset.

## Dataset Source
- **Platform**: Kaggle
- **Title**: OkCupid Profiles
- **Link**: [https://www.kaggle.com/datasets/andrewmvd/okcupid-profiles](https://www.kaggle.com/datasets/andrewmvd/okcupid-profiles)
- **Original Source**: Kim, A. Y., & Escobedo-Land, P. (2015). *OKCupid Data for Introductory Statistics for Data Science Courses*. Journal of Statistics Education, 23(2).

## Instructions for Local Setup
1. Download `okcupid_profiles.csv` (approx. 137 MB) from the Kaggle link above.
2. Place the downloaded file into this `data/` directory:
   ```
   data/okcupid_profiles.csv
   ```
3. Run the analysis notebook in `notebooks/okcupid_community_detection_louvain.ipynb`. The notebook will automatically detect the dataset path.

> **Note**: `okcupid_profiles.csv` is ignored by Git (`.gitignore`) to comply with GitHub's 100 MB file size limit.

