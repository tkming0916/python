# 🐳 データサイエンス用のPython環境をDockerで構築した
完全に自分のためのメモ的なリポジトリ．

2023年度にビルドした環境を再構築した際に，うまくビルドできなくなっていたので備忘録がてら残しておく．

# 📦 インストール済みパッケージ
データサイエンスに必要なものは入れたつもり
- ipykernel
- numpy
- pandas
- matplotlib
- japanize-matplotlib
- scikit-learn
- tensorflow

# 🚨 注意
tensorflowのインストールのために，明示的に"libhdf5-dev"をインストールしておく必要があるみたい．．．
Dockerファイルに書いているけど，`RUN apt-get update && apt-get install -y libhdf5-dev`で対応．
