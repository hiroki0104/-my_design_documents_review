# テーブル定義書2
## 全体
- 

## admins
- 接頭語adminがいらない
- PKのINDEXにまるがない

## users
- 接頭語userがいらない
- lやfなどの略語を使用しない
- 退会ステータスは[is_active]のようなカラム名にする
- 退会ステータスはboolean型で良い

## ships
- 接頭語shipがいらない
- PKのINDEXにまるがない

## products
- 接頭語productsがいらない
- シングル名/アルバム名のカラム名は[title]で良い
- 在庫数カラムはいらない
- 在庫ステータスカラムはいらない
- deleted_atカラムを追加する

## discs
- 接頭語discがいらない
- FKは単数形にする

## songs
- 接頭語songsがいらない
- 曲名は[name],[title]などの方が良い

## labels
- 接頭語labelがいらない
- レーベル名は[name]などの方が良い

## artists
- 接頭語artistがいらない
- アーティスト名は[name]などの方が良い

## genres
- 接頭語genreがいらない
- ジャンル名は[name]などの方が良い

## cart_items
- テーブル名にスペースがある
- PKはidで良い
- FKは単数形にする
-  購入枚数のカラム名にスペースがある
- PKのINDEXにまるがない

## sell_details
- PKはidにする
- 商品IDのFKにまるがない、FKは単数
- カラム名はorder_detailsなどの方が良い
- sellsとのFKがない
- 小計金額カラムを追加する

## sells 
- カラム名はordersなどの方が良い
- PKはidだけで良い
- PKのINDEXにまるがない
- 購入詳細IDはいらない
- 支払い方法のカラム名が不適当
- totalではなく[total_price]などの方が良い

# 注意
* マークダウン形式で記入してください。
* 全体を通しての指摘事項の場合、テーブル名の部分を「全体」「共通」などとしてください。
