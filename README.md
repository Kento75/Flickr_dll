# Flickr_dl
Flickr APIを使用した画像取得スクリプト

*****
### 事前準備
・Flickr APIに登録して、APIキーとシークレットキーを取得する。


・APIキーとシークレットキーをスクリプト内に追記する。

```python:image_dl.py
from flickrapi import FlickrAPI
from urllib.request import urlretrieve
from pprint import pprint
import os
import sys
import time

# ↓APIキーを設定
key = ''
# ↓シークレットキーを設定
secret = ''

# 省略
```

・下記コマンドを実行してPythonライブラリ取得する。

　　pip install -r requirements.txt


*****
### 実行
・下記コマンドを実行すると、画像保存先(./images/{検索ワード})に対象の画像が保存される。

　　python image_dl.py {検索ワード} {取得枚数}

