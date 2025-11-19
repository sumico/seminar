ダミーのテキストデータ（レビュー文）＋数値データ（年齢・所得・予算・購入点数・サイト滞在時間・割引利用率）を生成し、消費者志向（Price‑Sensitive / Eco‑Conscious / Brand‑Loyal / Convenience‑Seeker）をマルチモーダル分類

**構成**

テキスト特徴量: TfidfVectorizer（ユニグラム＋バイグラム）

数値特徴量: StandardScaler（標準化）

特徴結合: ColumnTransformer（テキスト＋数値を一つの特徴行列へ）

分類器: LogisticRegression (multinomial, solver='saga')

評価: 5分割の層化CV（Accuracy & Macro‑F1）、テストセット評価、混同行列

説明可能性: クラスごとの上位TF‑IDF語、数値重み（係数）を出力

成果物: 生成データ（CSV）と学習パイプライン（pickle）を保存

---

Generates dummy text + numeric data and trains a simple, explainable multimodal classifier to predict consumer orientation (Price‑Sensitive / Eco‑Conscious / Brand‑Loyal / Convenience‑Seeker).

**Structure**

Text features: TfidfVectorizer (uni/bi‑grams)

Numeric features: StandardScaler

Feature fusion: ColumnTransformer (concatenate text + numeric)

Classifier: LogisticRegression (multinomial, saga)

Evaluation: Stratified 5‑fold CV (Accuracy & Macro‑F1), test set metrics, confusion matrix

Explainability: Top TF‑IDF terms per class + numeric feature weights (coefficients)

Artifacts: Saves synthetic dataset (CSV) and trained pipeline (pickle)

---
