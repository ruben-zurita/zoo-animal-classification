# Animal Classification — Decision Tree vs. Random Forest vs. XGBoost

Comparing three tree-based models to classify animals into 7 classes (mammal, bird, reptile, fish, amphibian, insect, arachnid) from 16 biological attributes.

![Python](https://img.shields.io/badge/Python-3.11-blue) ![scikit--learn](https://img.shields.io/badge/scikit--learn-trees-F7931E) ![XGBoost](https://img.shields.io/badge/XGBoost-boosting-189FDD)

## What I did
- **Cleaning:** loaded the raw headerless file, dropped the name column, moved the target to the front, assigned readable column names and mapped numeric classes to labels.
- **EDA:** class distribution (heavily imbalanced: mostly mammals, amphibians only 4 %).
- **Models:** Decision Tree (with tree visualization), Random Forest (tested how many trees are needed — no gain after ~6), and XGBoost.
- **Interpretability:** feature importance from Random Forest and XGBoost.

## Results
| Model | Test accuracy |
|---|---|
| Decision Tree | 92 % |
| **Random Forest** | **96 %** |
| XGBoost | 95 % |

Random Forest had the best precision and recall. Minority classes are the hardest to predict simply because there are very few examples of them.

## How to run
1. Download `zoo.data` from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/111/zoo) into `data/`.
2. `pip install -r requirements.txt` and open `zoo_classification.ipynb`.

---
**Ruben Zurita Calzada** · Data Science Engineering student, Universidad Autónoma de Querétaro · [LinkedIn](https://www.linkedin.com/in/ruben-zurita/)
