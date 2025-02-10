# Dockerfile
FROM python:3.9-slim

# 作業ディレクトリ
WORKDIR /workspace

# システムパッケージの更新 & 必要パッケージインストール
# prophet (旧 fbprophet) や statsmodels 等はビルドに C++コンパイラ等が必要
RUN apt-get update && apt-get install -y --no-install-recommends \
    git \
    build-essential \
    python3-dev \
    && rm -rf /var/lib/apt/lists/*

# requirements.txt をコンテナにコピー
COPY requirements.txt .

# Python ライブラリのインストール
RUN pip install --upgrade pip && \
    pip install --no-cache-dir -r requirements.txt

# デフォルトコマンド（Jupyter Notebookを起動）
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]
