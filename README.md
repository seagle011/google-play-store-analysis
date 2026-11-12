# Google Play Store analysis

This Python analysis explores a historical snapshot of Google Play listings and reviews. The notebook cleans the listings, compares ratings, prices and reported install thresholds, and joins listings to scored reviews to compare sentiment across free and paid apps.

## Results from the supplied snapshot

- Of 9,659 app records, 8,196 had usable ratings. Their mean rating was 4.17 out of 5.
- Median reported install thresholds were 100,000 for free apps and 1,000 for paid apps. These are lower bounds displayed by the data source, not exact install counts.
- The sentiment comparison matched 35,934 scored reviews to 816 apps, including only 9 paid apps. The scores are supplied by the dataset and the reviews are selected. This comparison cannot establish a difference in app quality.

## Run the analysis

- **Colab or Kaggle:** Upload `Play Store Analytics.ipynb`, enable internet access if necessary, and run all cells. If the CSVs aren't in the working directory, the notebook downloads them from a fixed revision of the original repository. In an offline session, put `apps.csv` and `user_reviews.csv` there instead.
- **Local Jupyter:** Run `python -m pip install -r requirements.txt` in your environment. Open the notebook from this folder and run all cells.

## Sources
- Data: [Lavanya Gupta, Google Play Store Apps](https://www.kaggle.com/datasets/lava18/google-play-store-apps), listed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). The notebook uses the CSV snapshots from the [original repository](https://github.com/seagle011/google-play-store-analysis).
