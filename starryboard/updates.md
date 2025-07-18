# Starryboard の更新情報

## [Starryboard](/starryboard/about)

## 対応予定

* v0.4.1~ 
  * 参照表示UI（別カット参照表示やウィンドウキャプチャ、外部画像取り込みなど）の見直し
* v0.5 参照表示を整理
* v0.6 カメラとレイヤーのアニメーション機能
* v0.7 シーン管理の強化とサウンド再生に対応
* v0.8 インポート対応、エクスポートの整理

## 更新履歴

### v0.4.10 

キャンバスの色選択の表示を見直して選びやすくした上で、レイヤー選択＋色選択を一括で行える「タグ別カラーパレット」を追加しました。

キャンバスページの変更点
* 変更：カラーパレットポップアップに自由な色選択表示を追加しました
* 変更：タグ別カラーパレットを従来のカラーパレットポップアップから削除し、キャンバス上に直接表示するよう変更しました
* 修正：ドロワーのアイテムメニューからドロワー設定を開こうとした際、指定したドロワーが表示されるよう修正しました
* 変更：ドロワーボタン上でマウスホイールを動かすことでドロワーを変更できるようにしました
* 変更：エピソード内カラーのカラーパレットの並べ替えに対応しました
* 変更：レイヤーアイテムに不透明度を変更するボタンを追加しました。ボタン上でマウスホイールを動かすか、ボタンをタップして表示されるスライダーを動かして変更できます
* 変更：カット切り替え後に選択中レイヤーのタグが維持されるようカットにレイヤーを自動的に追加するようにしました

設定ページの変更点
* 変更：ドロワー設定のペン先をボールペンに指定した時のペンサイズの幅の値を高さに反映できる設定を追加しました

その他の変更点
* 変更：エピソード作成時に自動作成されるドロワーを更新しました
  * 絵筆、太さが描写速度によって変わる動作を削除して太いペンのように変更しました
  * 新しくブラシペンを２種を追加しました。
* 修正：エクスポートページから動画コンテをエクスポートし、それをキャンセルした際にエラー表示されていた問題を修正しました

### v0.4.9

* 修正：キャンバスページを右クリックで移動させる際にポインターと移動がズレていた問題を修正しました。

### v0.4.6 ~ v0.4.8

ストア認証の調整作業でバージョン番号を使用。アプリはv0.4.5と同じです。

### v0.4.5

シリーズとエピソードの管理を一つページに統合しました。
シリーズエピソード一覧ページの機能は以下の通りです

* シリーズ（フォルダ）をツリービューによる一覧表示
* エピソードアイテムにカット数、再生時間、ファイルサイズを表示
* エピソードのカバー画像を表示できます
* エピソードを別のフォルダに移動できます

その他の変更点
* 修正：複数ウィンドウ表示が出来なくなっていた問題を修正しました

### v0.4.4

キャンバスページの変更点
* 修正：オニオンスキンの参照カットに未描写のベクターレイヤーが含まれるとオニオンスキンが表示できなくなっていた問題を修正しました
* 修正：オニオンスキンの範囲指定後にオニオンスキンを非表示にして、オニオンスキン対象の別カットに選択変更した上で再度オニオンスキンを表示するとオニオンスキンの参照表示が更新されていなかった問題を修正しました
* 更新：エクスポートボタンをウィンドウバーからページ内部に移動しました
* 修正：マウススクロールによるキャンバス拡大縮小時にマウス位置に応じたキャンバスの表示位置となるよう挙動を調整しました
* 修正：キャンバスを左右反転表示している際に、ジェスチャ操作によるキャンバスの拡大縮小が出来なくなっていた問題を修正しました
* 更新：キャンバスページにヘルプUIを追加しました。ウィンドウバーの？ボタンからページ内のボタンの説明を表示できる画面を呼び出せます

プレビューの変更点
* 更新：プレビュープレイヤーの操作ボタン類のレイアウトを変更しました
* 修正：プレビューを開くと同時に再生開始されるよう修正しました

リストページの変更点
* 修正：カットのサムネイル画像の枠線右側が表示されていない問題を修正しました
* 更新：プレビューボタンとエクスポートボタンをウィンドウバーからページ内部に移動しました

その他の変更点
* 更新：アプリ初回起動時にサンプルエピソードを作成し、キャンバスページで開く動作を追加しました
* 更新：エピソード作成時に動画コンテのエクスポート方法を追加するよう変更しました
* 更新：フィードバックフォームに英語版を追加しました
* 更新：ウィンドウバーにあるフィードバックボタンで表示できるポップアップ内のボタンを押しやすいよう整理しました
* 修正：アプリのストア情報に言語サポートに英語が表示されるよう修正しました
* 更新：各ページの背景色を調整しました



### v0.4.3

キャンバスページの変更点
* 更新：オニオンスキンの表示切替ボタンをキャンバスアクションリストに並べるよう変更しました
  * オニオンスキンボタンを押すと「表示するカット範囲」「不透明度」「表示タグ」「前方向・後方向の色指定」を変更できます
* 修正：キャンバスの初期表示位置を調整しました
* 修正：カットのキャンバスサイズを変更した際、各レイヤーの表示サイズに反映されていなかった問題を修正しました
* 修正：画面上部のカット一覧の高さを調節できるように。「設定ページ＞アプリ設定＞エピソード編集設定＞カット一覧の高さ」から変更できます
* 修正：レイヤー貫通動作（消しゴム・範囲選択）時にタグ未指定レイヤーを表示切替できるようにしました
* 更新：お絵描きセットをタグに対して複数登録できるよう変更しました

その他の変更点

* 更新：エピソード作成時のレイヤー画像形式をラスターに変更しました
* 修正：明るいテーマ表示時、カット表示時間ボタンやキャンバス上のセリフテキストなどが見づらくなっていた問題を修正しました
* 修正：キャンバスページ訪問時と離脱時の処理を効率化してページ移動時間を短縮しました
  1. カット番号の計算速度を効率化
  2. キャンバスページ到達時にシーン区切りの再生時間を集計する処理が二重実行されていた問題を修正
  3. 編集済みレイヤーの保存完了を待機する処理を削除

### v0.4.2

* 修正：レイヤー貫通（消しゴム・範囲選択）において選択中レイヤー以外の対象レイヤーに操作が反映されていなかった問題を修正しました
* 更新：リファレンスのウィンドウキャプチャと外部画像表示、別カットタグ別参照表示の表示基準をキャンバスからウィンドウに変更し、キャンバスの移動や変形に影響されなくなりました
* 更新：リファレンスの外部画像の表示状態をアプリ再起動後に復元するようになりました（ウィンドウキャプチャと別カットタグ別参照表示は非対応）
* 更新：リファレンスの表示アイテムが並び替えできるようになりました
* 修正：シリーズ一覧ページなどに動作しないエクスポートボタンが表示されていた問題を修正しました
* 更新：エラー通知の詳細表示を見やすくしました
* 更新：エラー通知をデフォルトで表示するように変更しました（インストール済みの場合は影響を受けません）
* 更新：アプリ設定にストアページを開くボタンを追加しました

### v0.4.0

* 更新：ロールとカテゴリによるレイヤー管理方法をシンプルなレイヤー管理＋タグの付与に変更しました。詳しくは次のリンクをご覧ください
  * [Starryboard v0.4からレイヤー管理がシンプルに変わります - note](https://note.com/tor4kichi/n/n1684dcf228eb)
* 修正：一部の環境で絵コンテエクスポートが動作しなくなっていた問題を修正しました
  * OS更新の影響でPDF出力時に指定フォントが見つからないエラーが原因でした
* 修正：キャンバスページのカットをアイテムメニューが開けなくなっていた問題を修正しました
* 更新：キャンバスページで、消しゴムや範囲選択の操作性を改善しました
* 更新：キャンバスページのダイアログやアクションのテキストをプレビュー再生時のようにキャンバス下部に表示するよう変更しました
  * ダイアログやアクションなどの表示切り替えボタンはキャンバス上部の色選択ボタンの右隣にある「３つの点ボタン」にある「キャンバスにテキストを表示」に移動しました
* 更新：プレビュー再生時に再生一時停止切替とコントロールUI表示切替を別々に操作するよう入力処理を変更しました
* 修正：接続カットの親を削除するとカット番号がズレるなど挙動が不安定になっていた問題を修正しました
* 修正：シーン区切りを追加・削除した時、正しいシーン番号が表示されない問題を修正しました
* 更新：絵コンテエクスポートに出力対象となるタグの選択肢を追加しました
* 更新：エピソード作成時のパラメータを保存するようにしました
* 更新：キャンバスとカット設定からレイヤー画像の保存形式を「ラスター」「ベクター」から選べるようにしました
* 修正：シリーズ一覧ページからフォルダを追加するボタンが機能しない問題を修正しました

*v0.4.1*

* 修正：リストページで追加・削除・並び替えの選択切替が表示されない問題を修正しました
* 修正：カット数が多数になるとカットのタイム変更処理が重たくなる問題を修正しました
* 更新：キャンバスページのレイヤーボタンのタグ名とレイヤー名の表示を二段まで許容するように
* 修正：消しゴムモード有効中にレイヤー貫通の切り替えボタンを2回押すと消しゴムモードが意図せず終了していた問題を修正しました
* 修正：ウィンドウキャプチャのメニューアイテムのローカライズ漏れに対応しました

### v0.3.10

* 修正：キャンバスページにて消しゴムと範囲選択が動作するよう修正しました
* ライトテーマで表示している際に、リストページの上部が黒い背景で表示されていた問題を修正しました

### v0.3.8

* 修正：エピソード作成時のキャンバスの高さの値が指定できなくなっていた問題を修正しました
* 修正：キャンバスページのアクション・セリフのテキストが１行目しか表示されていなかった問題を修正しました

### v0.3.7

フォルダ探索ページを廃止して、シリーズ一覧ページとエピソード一覧ページを追加しました

#### シリーズ一覧ページ

* ストレージ内の任意のフォルダをシリーズとして扱います
* デフォルトで存在する「作業用フォルダ」にはアプリローカル（アンインストール時に消えます）にあるエピソードと、アプリ外で.strdst拡張子ファイルを任意の場所から開いたエピソードが一覧表示されます
* フォルダのストレージ上からの削除には対応せず、アプリからフォルダへのアクセス権を解除する動作となっています

#### エピソード一覧ページ

* シリーズとして登録されたフォルダ内の.strdstファイルをエピソードとして扱います

#### キャンバスページ

* 変更：キャンバス画像の自動保存機能を追加しました
  * アプリ設定画面から自動保存の間隔指定できます
  * これまではレイヤー切り替えのタイミングで随時保存していました
  * 単一レイヤーを長時間編集している場合に保存されない状況を改善するものです
  
#### その他

* 変更：カットのサムネイル画像保存がより効率的に実行されるよう変更しました
  * カットごとに一つずつ画像ファイルを作成する方法から一つのデータベースファイルで全てのサムネイル画像を管理する方法に変更
* 修正：カットの接続状態変更時にカットのサムネイル画像が反映されないことがあった問題を修正しました


### v0.3.6

#### 設定画面

* 変更：設定画面をページ遷移を要する表示から各画面のポップアップ表示へと変更しました
* 変更：ショートカットキー設定を追加しました
  * 各画面の右上にある設定ボタン（歯車マーク）から設定を開いて、ショートカット設定を選択することで確認、編集できます
* 変更：アプリ設定・ショートカット設定のエクスポートとインポートに対応しました
  * 設定画面の右上の歯車マークから「設定を読み込む」「設定をファイルに保存」が選択できます

#### プレビュー画面

* 修正：プレビュー画面の範囲選択画面を開閉する度にメモリ使用量が増えていた問題を修正しました
* 変更：プレビュー画面の範囲選択画面に選択中範囲の開始と終了の位置にスクロールするボタンを追加しました

#### フィードバックUI

* 修正：タイトルバーのフィードバックUIに設定画面にあった手動エラー報告UIの表示オプションを移動しました
* 修正：フィードバックフォームのページを一つに統合した上で、フィードバックUIを整理しました

### v0.3.1

#### 変更
* プレビュー用の画面を１つにまとめてどのページからでも呼び出せるような形に変更しました

#### 修正 
* 塗りカテゴリなどのラスターレイヤーに対して範囲指定してコピー＆ペーストを実行しても貼り付けた画像が消えてしまっていた問題を修正しました

### v0.2.5
#### 修正
* キャンバスページを開いた時にキャンバスの縦横比が崩れることがあった問題を修正しました
* キャンバスページで、操作ごとに描写した線がチラツク問題を修正しました
* カットリストページのカットサムネイル画像が表示されないことがあった問題を修正しました
* キャンバスページでラスターレイヤー画像に対するUNDO操作が失敗するケースがあった問題を修正しました
* キャンバスページでロールを並べ替えした際にキャンバス上のレイヤーの並びか入れ替わっていなかった問題を修正しました

#### 変更
* キャンバスページのカテゴリ及びロールの各アイテムのアイテムメニューに設定を開くボタンを追加しました



### v0.2.2 ~ v0.2.4

#### 修正

* カット削除時に選択中カットの接続カット情報の更新に失敗していた問題を修正しました。
* キャンバスページでのタッチ操作時におけるキャンバス移動・拡大縮小・回転の各操作が動作していなかった問題を修正しました

#### 変更

* ロール参照表示に対応しました
  * 別カットのロールを右クリックして「参照を保持」を選んでから、参照表示したいカットを選んで永続参照部分の追加ボタンからロール参照を追加できます。
  * 参照元のロールの画像レイヤーを変更した場合、参照先の表示も更新されます
* プレビュー再生がより効率よく動作するよう調整しました

### v0.2.1 2024/12

#### 修正

* レイヤーカテゴリ設定ページでカテゴリ名を変更できなかった問題を修正しました
* レイヤーカテゴリ設定からカテゴリを編集時非表示に指定した後、キャンバスページ上のカテゴリ表示のペン形状がズレていた問題を修正しました
* レイヤーカテゴリ設定を変更するとキャンバスページのカラーパレットUIの色が表示されなくなっていた問題を修正しました
* カテゴリを編集時非表示に指定した後、消しゴム等が正常動作しなかった問題を修正しました
* キャンバスページを開いた際に、キャンバスの縦の比率が変わらないまま表示されていた問題を修正しました
* キャンバスページを開いた際に、キャンバスのデフォルト表示位置をカテゴリやロールのボタンなどを考慮した配置になるよう修正しました
* キャンバスページに左下のキャンバス変形補助UIにおいて、左右反転と上下反転のボタンが異なるアイコンとなるよう修正しました
* キャンバスページでベクターレイヤーをラスターレイヤーに変換操作後、動作が不安定化する問題を修正しました
* キャンバスページで画像を貼り付けた際、他の操作をしていない場合にレイヤーが保存されていなかった問題を修正しました
* プレビュー再生時に共有レイヤーに指定されたロールの描写情報が接続カットの子カットにおいて表示されていなかった問題を修正しました
* リストページでのカットの画像サムネイルが表示されないことがある問題を修正しました

#### 変更

* アプリ内で生じたエラーを確認するためのエラー報告UIを追加しました
  * アプリ設定から「手動エラー報告UIを表示する」をオンにすると表示されます
  * オンにするとエラー発生時に「エラー発生😱」ボタンが画面右下に表示されるようになります
* キャンバスページ内での消しゴム及び範囲選択の操作を選択中のロールに限定するよう変更しました

### v0.2.0 2024/11

#### 修正

* 設定ページにおいてサードパーティライセンス表記が表示されていなかった問題を修正しました
* 接続カットの共有レイヤーへの描きこみ内容がカット切り替え時に消えてしまっていた問題を修正しました
* 「共有レイヤーの編集中」表記がキャンバス左下のキャンバス変形補助UIのボタンと被って表示されていた問題を修正しました
* キャンバスページにおいてカット変更時に常に全レイヤーが保存されていたことによるカット切り替え
カット切替がスムーズに行われていなかった問題を修正しました
* キャンバスページのロールアイテムに「接続カット間でレイヤーを共有」を示す表示を追加しました
* キャンバスページを再表示した際にカラーパレットの色が表示されない問題を修正しました
* キャンバスページのカラーパレットUIにおいて選択中の色をわかりやすく表示するよう修正しました
* キャンバスページの選択中のカテゴリとロールを見やすくなるよう配色を調整しました
* アプリのタイトルバーのテキスト部分を掴んでウィンドウを動かせなかった問題を修正しました
* リストページにおいて、カットの追加や削除が操作できなかった問題を解消しました

#### 変更

* キャンバスページの描写用UIのレイアウトを左側に寄せるよう変更しました
* キャンバスページのカテゴリとロールの選択を１クリックで行えるよう整理しました
* カットの時間指定用ストップウォッチにおける計測操作と時間の反映操作を分けるよう変更しました
* キャンバスページでの表示上の上下反転、左右反転するボタンをキャンバス左下に追加しました（アイコンが同一のため見分けられない問題があります。修正予定です）

### v0.1.5 2024/11

#### 修正

* アプリセッション中にエピソードを閉じると同じエピソードが開けなくなる問題を修正しました
* 複数ウィンドウとして起動した際に既に使用中のエピソードが選択できていた問題を修正しました
* エピソード作成時に同名ファイルのチェックを行うように修正しました
* エピソードを複数選択して削除する操作が動作していなかった問題を修正しました
* キャンバスページから離脱するタイミングでカットのサムネイル画像が更新されるようにしました（アプリ終了時も含む） 
* キャンバスページのカット一覧からカット削除を選択した際に確認ダイアログを表示するようになりました
* たまにラスター画像レイヤーに対する変更がサムネイル画像に反映されなくなっていた問題を修正しました
* 消しゴム使用時に非対象レイヤーが半透明表示のままサムネイル画像を更新していた問題を修正しました
* Windows10端末で消しゴムアイコンが表示されていなかった問題を修正しました
* タブレットモード時にウィンドウ左上に常に戻るボタンを表示するようにしました
* プレビューページに透かし除去アドオン未購入時にウィンドウキャプチャ禁止となる旨の説明とアドオン購入UIを追加しました

#### 変更

* リストページとキャンバスページにて、内部的に利用しているカットリストアイテムをキャッシュするようにしました。読み込み時間の短縮、メモリの整理処理の削減などパフォーマンス改善が期待されます
* リストページのシーン一覧において、シーンごとのカット数と再生時間の小計を表示するようになりました
* キャンバスページのカット内の画像を保存をロールやカテゴリの選択変更時にも行うようにしました
* キャンバスを動かす操作を整理しました
  * マウスでは右クリックのみキャンバスを動かせます
  * タッチ操作時は動かせますが、設定から「タッチで描写」が有効な場合にはタッチでキャンバスは動かせません
  * ペン操作時はタッチでキャンバスを動かす前提ですが、マウス同様右クリック操作で動かせます
* キャンバス左下に配置されたキャンバス変形補助UIが一部動かせなかった問題を解消しました
  * 拡大縮小が操作できなかった問題を修正しました
  * 移動の操作がポインターホールド後にポインター移動を求める動作から、仮想パッド中心からのポインター位置の方向に押した時間だけ動くような動作へと変更しました
* 消しゴムモード時、キャンバス範囲外を２回連続でクリックすると消しゴムモードを終了する動作を追加しました
* 範囲選択モード時、選択範囲がゼロの選択を２回連続で行うと範囲選択モードを終了する動作を追加しました
* キャンバスページの選択中カットのカット番号表示部分をクリックすると、カット一覧におけるスクロール位置が現在カットを中心となるようスクロールする動作を追加しました


### v0.1.4 2024/11

#### 修正

* ラスター画像を範囲選択した後、キャンバスの上または左の端をまたいで移動させてからUNDO/REDOすると選択範囲の表示が崩れていた問題を修正しました
* キャンバスページを2回以降開いた時に範囲選択が出来なくなっていた問題を修正しました

### v0.1.3 2024/11

#### 修正

* ラスター画像の範囲選択が動作するように修正しました

#### 変更

* キャンバス変形用のボタンを画面左下に配置しました

#### 機能更新

* カテゴリを貫通する消しゴムと範囲選択に対応しました
* ベクター画像に対する消しゴム動作をラスター画像の円ベースに変更しました
* 簡易エクスポートに対応しました
  * キャンバスページのプレビュー範囲指定、プレビューページのリピート区間範囲を簡易エクスポートできます

### v0.1.2 2024/10

#### 修正

* エピソード作成時に自動で追加されるカテゴリ設定を調整しました
  * カテゴリ名をアプリの言語設定に合わせて表示するようにしました
  * ペンのサイズをキャンバスサイズに応じて変化するように
  * 筆圧を反映する設定をデフォルトでオフに変更
* レイヤーカテゴリ設定ページのカラーパレットを表示する設定のローカライズ漏れを修正しました
* レイヤーカテゴリ設定ページでカテゴリの指定を変更した場合にキャンバスページで設定が再読み込みされるようにしました
* キャンバスページでカット内のラスターレイヤーを編集していると、別カットに選択を移動しても前カットの描写状況が残ってしまっていた問題を修正しました
* 開いた状態のカラーパレットUIの色選択UIに明るさを変更するスライダーを追加


### v0.1.1 2024/10

このアップデートから更新情報でお伝えする際の「ページの呼称」を変更しました

* カット編集ページ → キャンバスページ
* カット一覧ページ → リストページ

以下は変更ありません

* フォルダ探索ページ
* エクスポートページ
* プレビューページ
* 設定ページ

#### 修正

* 動画コンテ出力時にカットの再生時間がゼロの場合に出力に失敗していた問題を修正しました
* チャプター結合用のbatファイル内に日本語等が使われていると実行に失敗していた問題を修正しました
* エピソードにシーン区切りが無い場合に動画用チャプターテキストを出力しないよう変更しました
* キャンバスページのキャンバスズーム切り替えボタンが白背景のキャンバスと同色で見えなくなっていた問題を修正しました
* アプリが管理していないフォルダから.strdstファイルを起動するケースのために.strdstファイルの作業用ファイルをテンポラリファイルに出力するように変更しました
* キャンバスページのプレビュー範囲指定のショートカットボタン２つが名称と動作が互い違いになっていた問題を修正しました
* キャンバスページでキャンバスを拡大表示した際にカット一覧など他の表示を覆ってしまう問題を修正しました
* キャンバスページにてカット一覧を表示サイズを変更する区切り線がキャンバス背景と同色で見づらかった問題を修正しました

#### 機能更新

* キャンバスページのレイヤー及びカテゴリの選択をそれぞれ別々のボタンから変更するようにしました
* キャンバスページのカット一覧の下にあった各種ボタン類のレイアウトを変更しました
  * カット番号の表示、１カットずつの移動、カットのタイム表示、テキスト編集ボタンが表示されるようになりました
  * リファレンスやキャンバスサイズ変更などの大きな機能切替に当たる操作は右側の「点３つのボタン」に格納しました
* 「塗り用カラーパレットを表示する」が有効なレイヤーカテゴリを選択した時に色選択が表示されるようになりました
* リストページとキャンバスページの表示キャッシュを有効化し、ページの移動が軽快に行われるように調整しました


### v0.1.0 2024/10

#### 修正

* プレビュー再生時にCPU利用率が想定より高くなっていた問題を修正しました
* カット編集ページを開いた時に、キャンバスやカット一覧の表示ズレが視認できていた問題を修正しました

#### 機能更新

* プレビューページを追加しました
  * カット一覧ページ、カット編集ページの画面上部に表示された再生ボタン（横向きの三角形が表示されたボタン）からプレビューページを開くことができます
  * プレビューをメインに行う画面で指定区間のリピート再生に対応
* カット編集ページのプレビュー範囲指定の方法を刷新しました
  * 範囲指定開始ボタンを押したらカット一覧から２つのカットを選択する形に変更しました
  * 合わせてカット一覧のスクロール操作に対してプレビュー範囲が追従する動作は削除しました


### v0.0.9 2024/09

#### 修正

* カット編集ページのオニオンスキンは「リファレンス」タブに移動しました
* カット削除やカット接続切替のタイミングで内部情報が壊れ、エピソード読み込みが出来なくなっていた問題を軽減しました
* すべてエクスポート時に各エクスポート方法の有効・無効切替が反映されていなかった問題を修正しました
* エクスポート方法「台本」をすべてエクスポートに含めていた場合に、台本のみエクスポート処理が開始しない問題を修正しました
* エクスポート方法「動画の字幕」の対象指定のデフォルト値をActionからDialogに変更しました

#### 機能更新

* エクスポート方法に「動画用チャプターテキスト」を追加しました
  * 同時にffmpegを利用した動画とチャプターの結合用Batファイルを出力できます
  * ffmpegは別途インストールが必要です [詳しくはこちら](/starryboard/features/merge-video-and-chapters)



### v0.0.8 2024/09

#### 修正

* シーン区切りが削除できなかった問題を修正しました
* カット一覧ページで、接続カットの途中にカットを追加できるように修正しました
* カット一覧ページで、シーン区切りのジャンプスクロールがスムーズに行われるよう修正しました
* カット一覧ページとカット編集ページのカットアイテムのメニュー項目の表示が共通のものになるよう調整しました
* カットを接続する際、前後どちらのカットにもカット区切りがあるとカット区切りが削除されずにエピソードが開けなくなる問題を修正しました


### v0.0.7 2024/09

#### 修正

* 接続したカットの子カットを削除した際に削除カットの情報が正常に削除されいなかった問題を修正しました
* カット一覧ページのシーン区切りジャンプ機能が一部機能しなくなっていた問題を修正しました

### v0.0.6 2024/09

#### 機能更新

* カットに対してシーン区切りを指定する機能を追加しました
  * カット一覧ページのカット番号部分から「シーン区切りに指定」を選択すると指定できます
  * カット一覧ページの右側にある三本線のボタンからシーン一覧を表示でき、シーンの選択と削除を行えます

#### 修正

* カット削除時にエピソードファイルからカット関連データを除去できていなかった問題を修正しました
* カット一覧ページにおける子カットのカット番号が表示されていなかった問題を修正しました
* カット一覧ページでカットの個別追加しようとした際に追加位置がズレていた問題を修正しました
* カット一覧ページ上部の表示がスクロールしていると滲む問題を修正しました

### v0.0.5 2024/09

#### 機能更新

* 台本エクスポート時に話者名とセリフを分離して表示できるようになりました
  * [詳しい指定方法はこちら](https://tor4kichi.github.io/starryboard/features/features_v0)

#### 修正

* アプリ内の表現として「シーン」を「エピソード」に置き換えました
  * 今後、エピソード内のカットをシーン分割する機能実装を予定しているため文言を整理するものです
* 台本エクスポート時に、Cutやダイアログの表示項目名にシーン設定の入力内容が反映されていなかった問題を修正しました
* エピソード一覧ページから設定ページを開いたときに、エピソードファイルを開いていないのにエピソード関連の設定タブが表示されていた問題を修正しました


### v0.0.4 2024/09/11

#### 新機能

* 台本エクスポートに対応しました
* アプリ設定から表示テーマを変更できるようになりました
* カットのキャンバス編集中、消しゴム使用時に対象レイヤー以外を半透明表示にする機能を追加しました

#### 修正 

* レイヤーカテゴリのラスター指定が反映されておらず全てベクター画像で作成されていた問題を修正
* カットのキャンバス編集中、消しゴム使用時に範囲円がポインターとズレていた点を修正
* カット編集ページのダイアログやアクションのテキストボックスにフォーカスがある状態で別カットを選択したりページ移動した際に、編集中テキストが保存されていなかった問題を修正
* ライトテーマ時に画面の一部が見づらくなっていた問題を修正



### v0.0.3 2024/08/31

* 英語の翻訳を追加（日本語からの機械翻訳のため、ニュアンスが異なる可能性があります）
* Timeの変更単位に 1 以上を指定する機能を追加しました。アプリ設定ページから変更できます。デフォルトは 2 です
* エクスポートページにおける透かし除去アドオンが購入できるようになりました。あわせて透かし除去のお試し機能は削除しました

### v0.0.2 

* 2024/08/17 初リリース
