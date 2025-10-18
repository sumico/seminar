page 1

不均衡データ（imbalanced data）

<img width="402" height="243" alt="image" src="https://github.com/user-attachments/assets/1de41e9f-58be-40d0-819d-81b68b8e38fe" />

Source: https://book-read-yoshi.hatenablog.com/entry/2021/07/31/imbalanced_data_smote

---
page 2

**不均衡データ**では、一方のクラス（例：ポジティブ／ネガティブ）が極端に少ないため、
モデルが多数派クラスばかりを正解と予測してしまい、少数派クラスを正しく学習できなくなる可能性がある。
その結果、精度が高く見えても実際の性能（特に少数派クラス検出能力）が低下する。
したがって、バランスを取る処理（例：サンプリング、重み付けなど）が必要。


不均衡データ（imbalanced data）への主な対処方法

* オーバーサンプリング（Oversampling）：少数クラスのデータを増やす。
* アンダーサンプリング（Undersampling）：多数クラスのデータを減らす。

分類問題では「undersampling ≒ (おおよそ等しい) downsampling」ですが、
文脈（特に時系列や画像処理）によっては「意味が異なる」ことに注意が必要。

画像処理での意味

Downsampling
→ 画像の**解像度を下げる（画素数を減らす）**処理。
例：512×512 → 128×128

Undersampling
→ サンプリング点を間引くという信号処理的な意味を持ち、
画像全体を縮小する downsampling とは異なる。

---
page 3

In **imbalanced data**, one class (e.g., positive/negative) is much smaller than the other.
This causes the model to favor the majority class and fail to learn the minority class properly.
As a result, the model may show high accuracy but poor real performance, especially in detecting rare cases.
Therefore, balancing techniques (e.g., sampling, weighting) are needed.

* Oversampling: Increase minority class samples.
* Undersampling: Reduce majority class samples.

In classification tasks, “undersampling” ≒ (nearly equal) “downsampling”,
but their meanings can differ depending on the context,
especially in time-series or image processing.

In image processing

Downsampling
→ Reducing spatial resolution, e.g., 512×512 → 128×128 pixels.

Undersampling
→ Refers to insufficient sampling of data points (in signal theory),
not exactly the same as resizing or reducing image resolution.

---

