# psemi-flask-sample
P講習 Flask講義用リポジトリ

## 起動方法
1. 仮想環境の作成・アクティベート
```
python3 -m venv venv
(Mac) source ./venv/bin/activate
(Windows) . venv/Scripts/activate
```
2. 依存環境のインストール
```
pip install -r requirements.txt
```

3. (初回起動時のみ) DBのセットアップ
```
python3
>>>from app import app, db
>>>with app.app_context():
...    db.create_all()
```

4. アプリ起動
```
python3 app.py
```

## 動作確認履歴
- 2024/12/18
  - python 3.12.6
