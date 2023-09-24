# Food Review Recommender

## プロジェクト概要

- Amazon Fine Food Reviewsデータセットを用いて、分析、モデル構築、データとモデルのライフサイクル管理等を行います。

## 利用技術

### ライブラリ

- PySpark
- MLflow
- DeltaLake
- DVC

## 項目

1. EDAと前処理: データの可視化を通じて、前処理の方法を検討します。
2. DVCによるデータのバージョン管理: 以下のコマンドにより、データファイルのバージョン管理を行います。

    ``` bash
    dvc add data_directory/
    git add data_directory.dvc .gitignore
    git commit -m "Add raw data"
    dvc push -r local
    ```

3. 感情分析モデルの開発: ユーザーの感情に基づいたレビューを提供
4. モデルのバージョン管理:  MLflowを使用して構築したモデルのバージョンを管理
5. トピックモデリング: 主要なトピックやテーマを特定し、それに対するユーザーの意見を理解
6. 推薦システム: ユーザーの好みに合わせて製品を推薦
7. ユーザーの専門知識レベルの推定: ユーザーのレビューからその専門知識レベルを推定
8. 時系列解析: レビュートレンドの予測

## データセット

- [Amazon Product Reviews](https://www.kaggle.com/datasets/saurav9786/amazon-product-reviews)
- このデータセットはKaggleで利用でき、1999年から2012年までの約560,000件のレビューが含まれています。

## Architecture Diagram

作成中
