# Webサイト 2kg.jp 管理用リポジトリ

* OS
  * Windows 10 64bit
* Python
  * Python Embeddable
    * https://www.python.org/downloads/windows/
    * https://www.python.org/ftp/python/3.9.1/python-3.9.1-embed-amd64.zip

## 手順
* Pythonの公式サイトからWindows用embeddable Pythonインタプリタをダウンロード
  * 公式サイト
    * https://www.python.org
  * ダウンロードするファイル
    * https://www.python.org/ftp/python/3.9.1/python-3.9.1-embed-amd64.zip

* zipファイルをpython-3.9.1フォルダに展開し、元のzipファイルは削除

* 環境変数設定
  * 環境変数設定用のバッチファイルを配置
    * ```setenv.bat```
    * ```cmd4python.bat```

* pip設定
  * 参考サイト
    * [3.9. モジュールの検索 — Python 3.9.1 ドキュメント](https://docs.python.org/ja/3/using/windows.html#finding-modules)
  * 事前作業
    * モジュール検索PATH制限の解除のために```python39._pth```をリネーム
      * ```ren .\python39._pth .\python39._pth.bak```
    * pipインストーラファイルのダウンロード
      * https://bootstrap.pypa.io/ から```get-pip.py```をダウンロード
      * ```get-pip.py```を```python-3.9.1```フォルダに配置
  * pipインストール
    * ```cmd4python.bat```を実行しコマンドプロンプトを開く
    * カレントディレクトリが```python-3.9.1```となっていることを確認の上で下記コマンドを実行
      * ```python.exe get-pip.py```

## 参考サイト
* [Windowsでpythonを使う/配布する時に便利！Python embeddable package使い方 - ひつじ工房](https://hituji-ws.com/code/python/python-emb-usage/)
* [Python Embeddableの使い方](https://engineer-milione.com/programming/python-embeddable.html#1)
