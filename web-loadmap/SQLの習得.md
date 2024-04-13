# SQLの習得

データベースを操作するにあたって必要な問い合わせ言語であるSQLを習得しよう。

## ゴール

任意のDBMSにて、以下の4種類の操作を実行してみよう。

- 挿入
- 更新
- 削除
- テーブル作成

## 書籍

* [スッキリわかるSQL入門 第3版 ドリル256問付き\! \(スッキリわかる入門シリーズ\) \| 中山 清喬, 飯田 理恵子, 株式会社フレアリンク \|本 \| 通販 \| Amazon](https://www.amazon.co.jp/%E3%82%B9%E3%83%83%E3%82%AD%E3%83%AA%E3%82%8F%E3%81%8B%E3%82%8BSQL%E5%85%A5%E9%96%80-%E7%AC%AC3%E7%89%88-%E3%83%89%E3%83%AA%E3%83%AB256%E5%95%8F%E4%BB%98%E3%81%8D-%E3%82%B9%E3%83%83%E3%82%AD%E3%83%AA%E3%82%8F%E3%81%8B%E3%82%8B%E5%85%A5%E9%96%80%E3%82%B7%E3%83%AA%E3%83%BC%E3%82%BA-%E4%B8%AD%E5%B1%B1/dp/4295013390)

入門にはもってこい！
「達人に学ぶ」シリーズが非常に有用だが、ちょっと難しいのでいったん置いておく。

* [これからはじめる MySQL入門 \| 小笠原 種高 \|本 \| 通販 \| Amazon](https://www.amazon.co.jp/%E3%81%93%E3%82%8C%E3%81%8B%E3%82%89%E3%81%AF%E3%81%98%E3%82%81%E3%82%8B-MySQL%E5%85%A5%E9%96%80-%E5%B0%8F%E7%AC%A0%E5%8E%9F-%E7%A8%AE%E9%AB%98/dp/4774197599/ref=tmm_other_meta_binding_swatch_0?_encoding=UTF8&dib_tag=se&dib=eyJ2IjoiMSJ9.dFy3AB2cKsarqdeB2thZCQ8rkLMqzMllsMAy3mocuhPT3imS5y_tKwbPsLRrDfUMUzFb3-UKlfLSXOsNjn8Fs_LZ9IqXu22Eqc9ozOnYXoFv727hIiuhr3sgkJxdfFL1YMPPNKyxOi1p8_YKjuXdqbSgtxju1VwiTQY8MlSugiULJydH_xasp6RUtor6cWYIf1xDqyK3h1713hV7mZK4kPweT3cyoJkbI0dYXlfNs9g.hKoyFzkwJSN3EaYyt3lYKh7wSHlaq4bxjch-wmOgwCM&qid=1713005739&sr=1-11)

好きなDBを利用して構わないが、ここではMySQLを挙げる。
こちらを実際に読んだことがあるが、入門には問題なし。

## 押さえておきたいこと

- データベースへの問い合わせ。条件検索をよく使うので、WHERE句はちゃんと覚える。
- 設計技法。概念設計・論理設計・物理設計は押さえておきたい。
- トランザクション。ロックについては、すぐには分からなくとも概要はつかんでおきたい。
- データベースを用意できるようなら、サーバーを立ち上げるのもよい。
- DBMSのアカウント管理。読み取り専用ユーザーなどを作ってみよう。
- 高速化の手段については、すぐにはわからなくとも把握はしておきたい。
  - 例えば、インデックス・パーティションなど。
- バインド変数などによるクエリの動的な生成方法も押さえたい。
  - 当然、アプリから発行するクエリは、検索条件などは入力値によって異なる場合があるため。

## 今は大変だが、なんとなく意識したいこと

- パフォーマンス。大量レコードがあるときに、それなりのレスポンスを出せるか？
→難しい話だが、避けては通れない。