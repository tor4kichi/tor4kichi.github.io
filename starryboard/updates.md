# Starryboard の更新情報

## 対応予定

### vNext

* 画像の貼り付け時にカットが画像データを保持できるように
* 新しいカット一覧に表示方法（グリッドやテキストのみ）に対応
* 動画コンテの出力用キャッシュを随時生成するオプション
* シナリオのインポート

## 更新履歴

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
