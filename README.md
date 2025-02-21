![oasst1](image/oasst1_repo.png)

**Update:**  
- 2023/10/21  
自動翻訳によるコード関連データの翻訳誤り2000箇所程度を手動で修正しました。  

**<details><summary>修正イメージを表示</summary><div>**
  
- 修正前
```
もちろん！これは、Flask Webフレームワークを使用して文字列を提供する単純なAPIエンドポイントを作成するPythonスクリプトの例です。

フラスコ輸入フラスコから

app = flask（__name__）

@app.route（ '/'）
def hello_world（）：
    「こんにちは、世界！」を返します

__name__ == '__main__'の場合：
    app.run（）

このスクリプトでは、最初にフラスコモジュールからフラスコクラスをインポートします。次に、__Name__変数を使用してアプリケーションの名前を指定するフラスコクラスの新しいインスタンスを作成します。
```
- 修正後
```
もちろん！これは、Flask Webフレームワークを使用して文字列を提供する単純なAPIエンドポイントを作成するPythonスクリプトの例です。

from flask import Flask

app = Flask(__name__)

@app.route('/')
def hello_world():
    return 'Hello, world!'

if __name__ == '__main__':
    app.run()

このスクリプトでは、最初にフラスコモジュールからフラスコクラスをインポートします。次に、__Name__変数を使用してアプリケーションの名前を指定するフラスコクラスの新しいインスタンスを作成します。
```

</div></details>

# oasst1-89k-ja
OpenAssistant のオープンソースデータ OASST1 を日本語に翻訳したデータセットになります。  
日本語大規模言語モデルの作成にご活用下さい。なお、データセットのライセンスは、 Apache 2.0 になります。  
日本語への翻訳には Google 翻訳を使用しました。

「ng_translation」カラムは、日本語翻訳に失敗したかどうかを示すカラムになっており、「1」となっている場合は翻訳に失敗しており、この場合は翻訳前のテキストがそのまま「text_ja」に入っています。

**データセット内で翻訳誤り、誤字、脱字、文脈の違和感等あるレコードがあった場合はPull requests いただけると助かります（英語弱者なのでPRは日本語で大丈夫です）。**  
「use_deepl」が「0」になっているものはすべてGoogle翻訳で日本語翻訳されています。マイナーな言語だと日本語翻訳の精度が怪しいと感じる部分がありますが、こういったデータはDeepLでの翻訳に差し替えるだけで改善するものもあると思っています（DeepLでの翻訳に差し替えた場合は「use_deepl」を「1」にしてPRしてもらえると助かります）。
  
huggingface上のデータセットも定期的に更新しますが、レポジトリから最新ファイルをダウンロードして使いたい場合は concat_json.py を使用してひとつのjsonファイルに結合してご利用下さい。

**huggingface**  
https://huggingface.co/datasets/kunishou/oasst1-89k-ja
