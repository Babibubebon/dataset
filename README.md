# メディア芸術データベース（ベータ版）データセット
## 1.概要

### 1.1. データセットの提供元

本データセットは、メディア芸術データベース（ベータ版）（以下「MADB」といいます。）<<https://mediaarts-db.bunka.go.jp/>>が提供しているメタデータを試験的に公開しています。

### 1.2. データセットの権利

メディア芸術データベース（ベータ版）データセットは、自由な二次利用が可能です。ただし、二次利用に際しては、次の事項へのご配慮をお願いいたします。これらのお願いは法的な契約ではありませんが、できる限りご留意の上でご利用くださるよう、ご協力をお願いします。

* データを編集・加工等して利用する場合は、それを行ったことを記載してください。編集・加工等を、元となる作品・原資料の作者や提供元が行なったかのような態様で公表しないようご留意ください。
* 当該データが自由に二次利用可能であることの表記を保持してください。
* 元となる作品や、その作者の名声を傷つける形での利用は行わないようご留意ください。また、元となる作品に関わる文化やコミュニティへの配慮を行ってください。
* 著作権以外の権利（著作者人格権、著作隣接権、肖像権、パブリシティ権、プライバシー権、商標権等）にも留意し、関連法令を遵守してください。
* 論文等に利用する場合には、先行研究や後続研究と比較を容易にするためメディア芸術データベースデータセットとバージョンの明記にご協力ください。

## 2.データセットの説明

### 2.1. データセットの概要について

* ファイル形式は、json-ld形式とturtle形式の2種類です。
* 情報資源分類ごとに、30種類提供しています。

### 2.1.1. 情報資源分類

* マンガ(CM)

|No|小分類ID|分野|大分類|小分類|
| :---------------: | :---------------: | --------- | --------- | --------- |
|1|cm101|マンガ|アイテム|マンガ単行本|
|2|cm102|マンガ|アイテム|マンガ雑誌各号|
|3|cm103|マンガ|アイテム|マンガその他|
|4|cm104|マンガ|コレクション|マンガ単行本シリーズ|
|5|cm105|マンガ|コレクション|マンガ雑誌|
|6|cm106|マンガ|コレクション|マンガ雑誌掲載履歴|
|7|cm107|マンガ|コレクション|マンガ作品|
|8|cm107|マンガ|アイテム|マンガ関連資料|

* アニメ(AN)

|No|小分類ID|分野|大分類|小分類|
| :---------------: | :---------------: | --------- | --------- | --------- |
|1|an201|アニメ|アイテム|アニメテレビ番組|
|2|an202|アニメ|アイテム|アニメビデオパッケージ|
|3|an204|アニメ|アイテム|アニメ関連資料|
|4|an205|アニメ|アイテム|アニメ劇場上映|
|5|an206|アニメ|アイテム|アニメその他|
|6|an207|アニメ|コレクション|アニメテレビレギュラーアニメシリーズ|
|7|an208|アニメ|コレクション|アニメテレビ単発（スペシャル）アニメシリーズ|
|8|an209|アニメ|コレクション|アニメビデオパッケージシリーズ|
|9|an210|アニメ|コレクション|アニメ劇場上映シリーズ|
|10|an211|アニメ|コレクション|アニメ作品|

* ゲーム(gm)

|No|小分類ID|分野|大分類|小分類|
| :---------------: | :---------------: | --------- | --------- | --------- |
|1|gm301|ゲーム|アイテム|ゲームパッケージ|
|2|gm305|ゲーム|コレクション|ゲームバリエーション|
|3|gm306|ゲーム|コレクション|ゲーム作品|
|4|gm317|ゲーム|アイテム|ゲーム関連資料|

* メディアアート(ma)

|No|小分類ID|分野|大分類|小分類|
| :---------------: | :---------------: | --------- | --------- | --------- |
|1|ma401|メディアアート|アイテム|メディアアート展示・実演|
|2|ma403|メディアアート|アイテム|メディアアートその他|
|3|ma411|メディアアート|アイテム|メディアアート関連資料|
|4|ma408|メディアアート|コレクション|メディアアート催事|
|5|ma408|メディアアート|コレクション|メディアアート作品|

* 分野横断(co)

|No|小分類ID|分野|大分類|小分類|
| :---------------: | :---------------: | --------- | --------- | --------- |
|1|co504|分野横断|キュレーション|責任主体|
|2|co505|分野横断|キュレーション|催事|
|3|co506|分野横断|キュレーション|トピック|

### 2.1.2. ファイル名

ファイル名は、metadata_[分野]-[大分類]\_[小分類ID]\_[出力形式].zipです。 

* 分野
   * マンガ：cm
   * アニメ：an
   * ゲーム：gm
   * 分野横断：co

* 大分類
   * アイテム：item
   * コレクション：col
   * キュレーション：curate
  
* 出力形式
   * turtle形式：ttl
   * json-ld形式：json

【単行本の例】metadata_cm-item_cm101_ttl.zip

### 2.2.　データセットのダウンロード先

 * 情報資源分類単位

　dataset/data/配下に登録してあります。

### 2.3.　データセットの詳細について

メディア芸術データベースデータ（ベータ版）メタデータスキーマ仕様書をご参照ください。

<<https://github.com/mediaarts-db/dataset/blob/main/doc/MADBメタデータスキーマ仕様書（Ver.0.9）.pdf>>

## 3.個別機能についての考え方


* Fork
    * ご自由にしていただいて構いません。
    
* Pull Request
    * 原則、Mergeいたしません。
    * 基本的に個別の返答は致しかねますが、いただいた意見はすべてに目を通し、今後の運営の参考にさせていただきます。

## 4.過去のバージョン情報

|公開日|バージョン|コメント　　　　　　　　　　|
| :---------------: | :---------------: | --------- |
|2021年1月25日| ver0.9|ベータ版の提供開始|
