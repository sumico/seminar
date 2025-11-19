**Sentinel-2（AWS Open Data）＋機械学習による時系列解析**

**Time-Series Analysis of Sentinel-2 (AWS Open Data) + Machine Learning**

登録不要、APIキー不要。Google Colab 上で実行可能 実験時間約30分間

No registration, no API keys. Runs on Google Colab. The experiment takes approximately 30 minutes.

このノートブックは、AWS Open Data に公開されている Sentinel-2 L2A 画像（Cloud-Optimized GeoTIFF：COG 形式）を、無料で利用できる Earth Search（STAC）API を通じて取得します。 指定した関心領域（AOI）に対して月次 NDVI を算出し、時系列を可視化し、さらに簡単な機械学習手法を用いて予測や異常検知を行います。

This notebook pulls Sentinel-2 L2A imagery published as Cloud-Optimized GeoTIFFs (COGs) on the Registry of Open Data on AWS, discovered via the free Earth Search (STAC) API. It computes monthly NDVI over your Area of Interest (AOI), visualizes the time series, and applies simple ML for forecasting and anomaly detection.

**References**

Sentinel-2 L2A COG dataset overview on AWS Open Data: https://registry.opendata.aws/sentinel-2-l2a-cogs/

Earth Search API (Element 84) description: https://element84.com/earth-search

Earth Search STAC API docs & endpoint: https://earth-search.aws.element84.com/v1/api.html

Reading COGs efficiently via HTTP with Rasterio: https://autogis-site.readthedocs.io/en/2020_/notebooks/Raster/read-cogs.html

---

<img width="1581" height="619" alt="image" src="https://github.com/user-attachments/assets/c589a259-5ea0-4505-9554-7b12c44f555e" />

---

<img width="921" height="704" alt="image" src="https://github.com/user-attachments/assets/770f8ef6-3de9-48dc-9369-30717454920e" />

---
