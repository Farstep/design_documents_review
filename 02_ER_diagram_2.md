# ER図2
## 全体
- 入荷情報を保持するテーブルがない。
- 配送先を複数保持するためのテーブルがない。
- 管理者テーブルとエンドユーザー、商品がそれぞれ関連づけられている。

## エンドユーザー
- 名前カラムがない。
- 主キーの名前が間違っている。

## 商品
- 在庫数カラムがある。
- ディスクIDという外部キーがある。
- 発売日カラムがない。
- ディスク枚数カラムがある。
- ステータスが何を意味しているか不明。（）に意味を書くのではなくカラム名にわかりやすい命名をする。

## ジャンル
- ジャンルというカラムの命名が適切でない。

## レーベル
- レーベルというカラムの命名が適切でない。

## ディスク
- 商品とディスクのテーブルのリレーションが逆になっている。
- トラックNo.カラムがある。
- ディスク名カラムがない。

## 曲
- ディスクと曲のテーブルのリレーションが逆になっている。
- トラックNo.カラムがない。

## カートアイテム
- PK（主キー）がない。
- 小計カラムがある。

## 購入
- 管理者側から見た役割で命名する方が適切であるから、テーブル名が適切でない。
- 宛名と郵便番号カラムがない。
- 購入日カラムがある。
- 発送状況を保持するカラムがない。

## 購入詳細
- 管理者側から見た役割で命名する方が適切であるから、テーブル名が適切でない。
- 購入テーブルと購入詳細テーブルのリレーションが逆。
- 商品テーブルとのリレーションがない。


**研修担当レビュー**
<font color="Red">再提出の際はこのレビューを残しておいてください。</font>

## 管理者
- [不足]  エンドユーザとのリレーションがある。
- [不足]  商品とのリレーションがある。

## 購入詳細
- [不足]  購入時価格を保持するカラムがない。
