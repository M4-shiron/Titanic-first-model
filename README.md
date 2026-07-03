# Titanic Survival Prediction

Kaggle「Titanic: Machine Learning from Disaster」の乗客データを使い、生存者を予測する二値分類プロジェクトです。

## Result

- Kaggle Public Score: **0.77990**
- 初期スコア **0.77511** から改善

## Approach

1. Ageの欠損値を中央値で補完
2. Sexなどのカテゴリ変数をone-hot encoding
3. SibSpとParchから **FamilySize** を作成
4. Random Forestで学習・予測
5. Kaggle提出用の submission.csv を出力

## Tech Stack

- Python
- pandas
- scikit-learn
- Jupyter Notebook / Kaggle Notebook

## Files

- titanic-machine-learning-from-disaster.ipynb — ベースモデル
- titanic-machine-learning-from-disaster (1).ipynb — 改善版ノートブック
- tensor-fiststep.ipynb — 学習過程の実験ノート

## What I Learned

欠損値処理、カテゴリ変数の数値化、特徴量エンジニアリングがモデルの精度に与える影響を実践的に確認しました。
