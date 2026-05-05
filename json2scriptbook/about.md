
# JsonToScriptBook 

台本製作作業を補助するアプリです。.jsonと.docxのファイルを組み合わせてカット番号、セリフなど繰り返しのレイアウトを自動的に処理し、文書ファイルを出力します。

拙作アプリ Starryboard から台本用JSONエクスポート機能とそれに合わせたテンプレートDOCXを提供しておりそれらの利用を前提としておりますが、テンプレートDocxとデータJSONのセットを用意すれば台本以外のどんな用途にも応用できます。

## ダウンロード

<a href="https://get.microsoft.com/installer/download/9nv7vnl63051?referrer=appbadge&cid=from_about" target="_self" >
	<img src="https://get.microsoft.com/images/ja%20dark.svg" width="200"/>
</a>

### 対応プラットフォーム

Windows11 （x86/x64/arm64）

## 使い方

### [Starryboard](../starryboard/about) を利用している場合

1. StarryboardのエクスポートからJSONを出力します
1. JSONエクスポートアイテムを展開して表示される「台本テンプレートを保存」からDocxファイルをローカルに保存します
1. JsonToDocxを起動して、DocxとJsonをセットします
1. JsonToDocxアプリの右側に「展開したDocx」の欄から処理されたDocxを取得できます。「コピー」または「名前を付けて保存」のボタンを押して任意の場所に保存します

<details>

<summary>Starryboard のエクスポート機能から分離している理由（ここをクリックして展開）</summary>

> .docx内のスクリプトを解釈するための DynamicExporesso というライブラリが、Starryboardをストア向けにパッケージングするための AOTビルド という工程で問題が生じさてしまうため、その解決方法としてAOTビルド抜きにストア向けパッケージを作成可能な WinUI3（WinAppSDK） をJsonToScriptBookの実装基盤として利用し、台本作成の動作を移行することとしました。



</details>

### 自前でDocxとJsonを用意する場合

[テンプレートのサンプルはこちらからダウンロードできます](https://1drv.ms/f/c/25a0f5ec5c869fb0/IgCsyMvJQapBQbitsVqZ6400AWg-R0EK7cUMz6I03TsYJ4E?e=eFE2fO)

ご自身で作った JSON のキー名に応じてテンプレートDocxに記述する変数を合わせるよう改変してください。

JSONに存在しないキー名がDocxファイルにある場合は、「展開したDocx」の欄にエラーメッセージが表示されます。エラーメッセージからどの変数がない（または誤字している）のか読み取れるかと思いますので、DocxやJsonを修正・保存して、エラー表示がなくなるまで修正を繰り返します。

アプリ内で選択中のDocxとJsonに対してファイル更新を自動検出するので都度変換ボタンを押す必要はありません。

#### テンプレート記述方法

詳細な記述方法は [DocxTemplater クイックリファレンス](https://github.com/tor4kichi/DocxTemplater#quick-reference-examples) を参照してください。


基本的には、`{% raw %}{{ }}{% endraw %}`（二重の波括弧）で変数を囲んで記述します。

##### 基本的な変数

JSONエクスポートで確認できる変数を、そのまま流し込むことができます。

記述例: `{% raw %}{{.CutNumber}}{% endraw %}` → `1`（カット番号に置換）

##### 全角変換オプション

変数名の後に :W を付けることで、半角英数字を全角に変換して出力します。

記述例: `{% raw %}{{.DialogText}:W}{% endraw %}`

##### 繰り返し処理（リスト）

JSON上で []（配列）となっているデータ（シーンやカットなど）は、# と / を使って繰り返し処理を記述できます。

開始: `{% raw %}{{#変数名}}{% endraw %}`

終了: `{% raw %}{{/変数名}}{% endraw %}`

記述例（シーンとその中のカットを繰り返す場合）:

```
{% raw %}{{#Scenes}}
  シーン番号：{{.SceneNumber}}
  {{#Cuts}}
    カット：{{.CutNumber}}
  {{/Cuts}}
{{/Scenes}}{% endraw %}
```

##### 条件分岐

変数の真偽値（true/false）や条件式によって、表示内容を切り替えることができます。

書式: `{% raw %}{{?{条件式}}} 真の場合 {{:}} 偽の場合 {{/}}{% endraw %}`

記述例: `{% raw %}{{?{.someVar > 5}}} 5より大きい {{:}} 5以下 {{/}}{% endraw %}`


#### おわり


