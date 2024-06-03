# ベースイメージを指定
FROM python:3.10

# pip アップグレード
RUN pip install --upgrade pip

# 必要なビルド依存関係をインストール
# libhdf5-devをインストールしないと，tensorflowがインストールできない
RUN apt-get update && apt-get install -y libhdf5-dev

# Pythonライブラリのインストール
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
