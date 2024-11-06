# 簡単なRAGシステムの構築方法
ChatGTPの既存LLMを活用してオリジナルのRAGを構築するプログラムになります。
# 事前に準備するもの
ChatGPTのアカウントとAPIKEY
RAGに学習させたい内容のテキスト
# 必要モジュールのインストール
requirements.txtに必要モジュールを記載しているので、以下コマンドを実行する
pip install -r requirements.txt
※requirements.txtがあるディレクトリで実行すること
# RAGが検索する外部データの作成
documents.txtファイルに事前に準備したRAGの検索させたい内容を記述する
# 設定ファイルの修正
config.jsonの"openai_api_key": "test"の"test"の部分を事前に取得したChatGPTのAPIKEYに書き換る。
その他、使いたいGPTのモデルなどに応じて各項目を変更すること。
# プログラムの実行
プログラムを実行するとコマンドプロンプトにテキスト入力が求められるのでそこでRAGが学習した外部データにかかわる質問をする。
→通常のChatGPTとは異なりRAGの学習内容が反映されていれば問題なく動作している。
