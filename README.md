This repo is for people who want to study time series analysis with python..

financial_timeseries_blog/
│── docker/                # Docker関連ファイル
│   ├── Dockerfile
│   ├── requirements.txt
│   ├── docker-compose.yml
│── notebooks/             # Jupyter Notebook (記事ごとに対応)
│   ├── 01_intro_to_timeseries.ipynb
│   ├── 02_basic_statistics.ipynb
│   ├── 03_stationarity_tests.ipynb
│   ├── 04_arima_model.ipynb
│   ├── 05_var_model.ipynb
│   ├── 06_garch_model.ipynb
│   ├── 07_lstm_for_timeseries.ipynb
│   ├── 08_feature_engineering.ipynb
│   ├── 09_backtesting_and_evaluation.ipynb
│   ├── 10_real_world_application.ipynb
│── blog/                  # 各章ごとの記事をMarkdownで保存
│   ├── 01_intro_to_timeseries.md
│   ├── 02_basic_statistics.md
│   ├── 03_stationarity_tests.md
│   ├── 04_arima_model.md
│   ├── 05_var_model.md
│   ├── 06_garch_model.md
│   ├── 07_lstm_for_timeseries.md
│   ├── 08_feature_engineering.md
│   ├── 09_backtesting_and_evaluation.md
│   ├── 10_real_world_application.md
│── src/                   # Pythonコード（モジュール化）
│   ├── data_loader.py      # データの読み込みと処理
│   ├── arima_model.py      # ARIMAモデル実装
│   ├── var_model.py        # VARモデル実装
│   ├── garch_model.py      # GARCHモデル実装
│   ├── lstm_model.py       # LSTM実装
│   ├── utils.py            # ヘルパー関数
│── data/                  # データ保存ディレクトリ
│   ├── raw/               # 生データ
│   ├── processed/         # 前処理後のデータ
│── .devcontainer/         # VSCode Dev Container 設定
│   ├── devcontainer.json
│── .github/               # GitHub Actions (CI/CD) 用設定
│── .gitignore
│── README.md
