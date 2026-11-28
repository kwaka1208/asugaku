# asugaku

このリポジトリは、Fireside（[kwaka1208/fireside](https://github.com/kwaka1208/fireside)）のテンプレートから作ったサイトです。本体の更新は、Actions の「Update Fireside」で取り込みます（[UPDATING.md](UPDATING.md)）。

## 変更の順番

- 機能や文書の変更は、先に Fireside 本体に入れる。asugaku には、Actions の「Update Fireside」で取り込む
- asugaku で直接変えてよいのは、`custom/` と、`.fireside-keep` に書いたファイルだけ。それ以外は、次の「Update Fireside」で Fireside の内容に置き換わる

## Claude に任せていること

- Fireside の変更は、指示がなくても asugaku に取り込む。asugaku に入れたくないときだけ、その旨の指示がある
- 進め方：Fireside で作業ブランチを作って PR を出し、CI が通ったらマージする。そのあと、asugaku の Actions「Update Fireside」を手動で実行し、できた PR（`fireside-update`）の差分と CI を確かめてマージする
- 両方のリポジトリで、PR のマージまで Claude が行ってよい
