---

このノートブックは、衛星画像を用いた作物種別のマッピングを深層学習によるセマンティックセグメンテーションで行う方法を解説しています。

具体的には、南アフリカのオレンジ川流域を対象とした Farm Pin Crop Detection Challenge のデータセットを利用し、Sentinel-2 のマルチタイムステップ画像（2017年1月～8月）からピクセル単位で作物種別を予測するタスクを扱います。

本チュートリアルでは以下の要素がカバーされています：

* U-Net アーキテクチャの実装（Keras Functional API 使用）

* 損失関数と評価指標：Sparse Categorical Focal Loss と精度、混同行列

* モデル保存と読み込みの方法

* セマンティックセグメンテーションの応用的理解と実装の習得

---

This notebook provides a tutorial on crop type mapping from satellite imagery using deep-learning based semantic segmentation.

It focuses on the Farm Pin Crop Detection Challenge, which provides ground truth crop type labels from multiple Sentinel-2 scenes captured between January and August 2017 in the Orange River region of South Africa. The task is to predict crop types at the pixel level.

Key concepts covered in this tutorial include:

* Implementation of the U-Net architecture (using Keras Functional API)

* Loss functions and metrics: Sparse Categorical Focal Loss, accuracy, and confusion matrix analysis

* Saving and loading Keras models

* Developing intuition and practical skills in semantic segmentation

---
