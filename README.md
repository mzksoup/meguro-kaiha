# 目黒区議会データ可視化（会派別議席数 × 会議日数）

このリポジトリでは、東京都目黒区が公開するオープンデータをもとに、以下の2つの指標をビジュアライズしています。

- 会派別の議席数の年度推移（折れ線グラフ）
- 年度別の会議日数（定例会＋臨時会の合計、棒グラフ）

## 🔍 使用データ

データ出典：東京都オープンデータカタログサイト
- [`kaihabetuuchiwake.csv`](https://spec.api.metro.tokyo.lg.jp/spec/t131105d0000000213-34fa3c9405e6432c3afc06c6de7e253c-0)：会派別議員数（年度別）
- [`kaisaikaisuu.csv`](https://spec.api.metro.tokyo.lg.jp/spec/t131105d0000000231-021931c59689943f303f5f1cfd1d4b5b-0)：議会開催回数・日数（年度別）


## 📊 使用技術

- [Chart.js](https://www.chartjs.org/)：グラフ描画
- [PapaParse](https://www.papaparse.com/)：CSV読み込み
- HTML / JavaScript（CDNベース、ビルド不要）

## 🚀 実行方法

ファイルをクローンまたはダウンロードし、`index.html` をブラウザで開くことで動作します。

```bash
$ git clone https://github.com/mzksoup/meguro-kaiha.git
$ cd meguro-kaiha
$ open index.html
```

## 補足
このリポジトリは、東京大学シビックテック・デザイン学創成寄付研究部門が運営する「デジタル技術と対話で創る未来 ーシビックテックを通じた参加の新しいかたちー」講座第5回「シビックテックを支えるオープンデータ・オープンソース」の課題提出物です。  
シビックテックの実践入門として、数十分程度で構築可能な「公共データの見える化」の実装例です。
