# テーブル定義書1
## 全体
- テーブル名が大文字から始まっている。
- テーブル名にはキャメルケースに似ているものを用いている。
- PK（主キー）がないテーブルがある。
- created_atカラム、updated_atカラムが全て「ユーザー登録日時」になっている。

## Admin
- テーブル名が複数形でない。
- PK(主キー)がない。
- カラム名の先頭に「admin_」が付いている。

## Users
- 姓の漢字が間違っている。
- 名前（姓）, 名前（名）, 名前(姓カナ), 名前(名カナ), 電話番号, メールアドレス, パスワードのカラム名に「user_」が付いている。
- 配送先カラムがある。

## Products
- FK（外部キー）がない。
- 「disc_id」カラムがある。
- ジャケット画像, シングル名/アルバム名に「cd_」がついている。
- 在庫数カラムがある。
- 在庫ステータスがある。

## Discs
- disc_idカラムの「disc_」が不要。
- FKである「product_id」の命名が適切でない。
- track_numカラムがある。
- ソート番号カラムがない。

## Songs
- songカラムの命名が適切でない。
- songカラムのデータ型がintegerになっている。

## Labels
- FK（外部キー）を持っている。
- labelカラムの命名が適切でない。

## Artists
- FK（外部キー）を持っている。
- artistカラムの命名が適切でない。
- artistカラムのデータ型がintegerになっている。

## Genre
- テーブル名が複数形でない。
- FK（外部キー）を持っている。
- genreカラムの命名が適切でない。
- genreカラムのデータ型がintegerになっている。

## Cart item
- FKである「product_id」の命名が適切でない。
- 「buy num」というカラムの命名が適切でない。
- subtotalカラムがある。

## Buy details
- 「Buy details」というテーブル名が適切でない。（テーブルの役割と異なっている）

## Buy
- 「Buy」というテーブル名が適切でない。（テーブルの役割と異なっている）
- 「buy_details_Id」というFK（外部キー）を持っている。
- stockカラムの命名がカラム説明と合致していない
- 支払い方法がのデータ型がstring型になっている。
- payカラムの命名が適切でない。




#レビュー

#Users
-郵便番号がinteger型
-電話番号がinteger型
-member_statusが何を意味しているか不明。
-member_statusが何を意味しているか不明。



#Songs
-曲順を管理するカラムがない


#Buy_details
-buy numは意味不明。スネークケースになってない。

