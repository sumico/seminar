Example Table: Structured Data with Missing Values
ID	Age	Gender	Income (USD)	Education Level	COVID-19 Risk Score
001	45	Female	58,000	Bachelor’s	0.72
002	53	Male	Missing	Master’s	0.81
003	Missing	Female	42,000	High School	0.54
004	36	Missing	75,000	Bachelor’s	0.68
005	29	Male	50,000	Missing	Missing


構造化データにおける欠損値

欠損値（missing value）とは、本来存在するはずのデータが観測・記録されなかった状態を指す。

構造化データ（表形式データなど）では、特定のセルに値が入力されていない状態（NaN、NULLなど）として表現される。

---
欠損値の対処方法

**1. 削除による対処**

欠損を含む行（レコード）を削除（listwise deletion）

欠損を含む列（特徴量）を削除（variable deletion）
→ データ損失のリスクが高く、小規模データでは注意が必要。

**2. 補完（Imputation）による対処**

平均値・中央値・最頻値による補完

グループ別平均や回帰モデルによる補完

k近傍法（KNN Imputation）や多重代入法（Multiple Imputation）

機械学習モデル（例：ランダムフォレストによる補完）

---
Missing Values in Structured Data

A missing value refers to a data point that should exist but is not observed or recorded.

In structured data (e.g., tabular data), missing values are represented as empty cells, NaN, or NULL.

---

Handling Methods for Missing Values

**1. Deletion-Based Methods**

Remove rows containing missing values (listwise deletion)

Remove columns with excessive missingness (variable deletion)
→ Risk of information loss, especially problematic for small datasets.

**2. Imputation-Based Methods**

Replace with mean, median, or mode values

Group-based or regression-based imputation

k-Nearest Neighbors (KNN) imputation or Multiple Imputation (MI)

Machine learning–based imputation (e.g., Random Forest Imputer)

---








