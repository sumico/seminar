目的：マーケティング文脈で、ダミーの製品データ（画像・レビュー文章・数値特徴）から 購入意向（buy=1/0） を予測する二値分類モデルを学習します。

モダリティ：

画像（ブランド名入りのシンプルな製品風画像）

テキスト（レビュー文テンプレート：great/good/average/poor/terrible の感情語を含む）

表形式（数値）：price（価格）、rating（評価）、discount（割引率）

モデル：PyTorch で レイト・フュージョン（late fusion） 構成。 画像用の小型 CNN、テキスト用 MLP（Bag-of-Words ベクトル入力）、数値用 MLP の3つのエンコーダ出力を結合して最終分類器へ入力します。

説明可能性：SHAP（KernelExplainer） を使って、表形式特徴（price/rating/discount） が予測（buy=1）に与える寄与度を可視化します。 ※マルチモーダルのうち、SHAP 解析では 画像とテキストをゼロ固定して、数値特徴の寄与にフォーカスします。

---

Purpose: In a marketing context, train a binary classification model to predict purchase intent (buy=1/0) from dummy product data (images, review text, numerical features).

Modalities:

Image (simple product-like image with brand name)

Text (review text template: containing sentiment words great/good/average/poor/terrible)

Tabular (numeric): price, rating, discount rate

Model: PyTorch implementation using a late fusion architecture. Combines outputs from three encoders—a small CNN for images, an MLP for text (using Bag-of-Words vector input), and an MLP for numeric data—before feeding them to the final classifier.

Explainability: Visualizes the contribution of tabular features (price/rating/discount) to the prediction (buy=1) using SHAP (KernelExplainer). *For SHAP analysis within multimodal data, images and text are zero-padded to focus on the contribution of numerical features.

---

