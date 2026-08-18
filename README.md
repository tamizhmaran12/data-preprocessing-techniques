# Data Preprocessing Techniques

A Jupyter notebook demonstrating five core data preprocessing techniques used in machine learning, implemented in Python with `pandas`, `scikit-learn`, `seaborn`, and `feature-engine`. Each technique is applied to a different real-world dataset and visualized before/after the transformation.

## 📓 Notebook

`Preprocessing_Assignment.ipynb`

## 🧪 Techniques Covered

| # | Technique | Dataset Used | Key Methods |
|---|-----------|--------------|--------------|
| 1 | **Normalization** | Wine dataset | Min-Max Scaling, Z-Score Standardization |
| 2 | **Binarization** | Titanic dataset | `sklearn.preprocessing.Binarizer` (age, fare) |
| 3 | **One-Hot & Label Encoding** | Tips dataset | `pd.get_dummies`, `sklearn.preprocessing.LabelEncoder` |
| 4 | **Imputation** | Titanic dataset | Mean, Mode (Most Frequent), and Median imputation via `SimpleImputer` |
| 5 | **Winsorization** | California Housing dataset | Outlier capping via `feature_engine.outliers.Winsorizer` |

## 📂 Datasets

The notebook expects the following CSV files to be present in the same directory (or update the paths accordingly):

- `1_Normalization_Wine.csv`
- `2_Binarization_Titanic.csv`
- `3_Encoding_Tips.csv`
- `4_Imputation_Titanic.csv`
- `5_Winsorization_CaliforniaHousing.csv`

## ⚙️ Requirements

```bash
pip install pandas numpy matplotlib seaborn scikit-learn feature-engine
```

## ▶️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```
2. Install the dependencies listed above.
3. Make sure all five dataset CSV files are in the same folder as the notebook.
4. Open and run the notebook:
   ```bash
   jupyter notebook Preprocessing_Assignment.ipynb
   ```

## 📊 What Each Section Does

- **Normalization** – Rescales `malic_acid`, `proline`, and `magnesium` columns using Min-Max scaling and Z-score standardization, then compares distributions with boxplots.
- **Binarization** – Converts `age` and `fare` columns from the Titanic dataset into binary categories using fixed thresholds (age ≥ 18, fare ≥ 50), visualized with histograms and count plots.
- **Encoding** – Applies one-hot encoding to categorical columns (`day`, `sex`, `smoker`) and label encoding to `time` and `day` columns of the Tips dataset.
- **Imputation** – Fills missing `age` values in the Titanic dataset using mean, mode, and median strategies for comparison.
- **Winsorization** – Caps extreme outliers in the `AveRooms` column of the California Housing dataset using quantile-based winsorization, with boxplots showing the effect.

## 🛠️ Tech Stack

- Python 3
- pandas / numpy
- matplotlib / seaborn
- scikit-learn
- feature-engine

## 📄 License

This project is for educational purposes as part of a data preprocessing assignment.
