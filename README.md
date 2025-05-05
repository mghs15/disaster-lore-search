# disaster-lore-search
自然災害伝承碑の簡易検索用ツール

* 国土地理院が提供している[自然災害伝承碑等の CSV データ](https://www.gsi.go.jp/bousaichiri/denshouhi_datainfo.html)の中身を簡易的に検索するためのツールです。
* まだ実装が甘い部分があるかもしれませんので、使用するときは**自己責任**でお願いいたします。

## 使い方

ツールの URL 

https://mghs15.github.io/disaster-lore-search/

1. まずは手元にCSV データ（国土地理院提供の CSV と同形式）を準備する。
    1. または、サンプルデータ（条件は後述）を利用することができます。
2. ツールを開いて、CSV データをアップロードする。
    1. または、「サンプルデータ」ボタンを押して、サンプルをロードする。
3. 各種条件を調整して、「絞り込み」ボタンを押す。

（参考）ヒートマップタイル

https://mghs15.github.io/disaster-lore-search/tilemap.html

※[自然災害伝承碑等の GeoJSON データ](https://www.gsi.go.jp/bousaichiri/denshouhi_datainfo.html)を使用

## 特長
* CSV の行全体や特定の列を対象として文字列検索（正規表現利用可）
* 種別ごとの絞り込みも可
* CSV （ヘッダー付き）で出力可能
* 地図への表示・範囲での絞り込みも可能

## Reference
* 自然災害伝承碑（国土地理院）https://www.gsi.go.jp/bousaichiri/denshouhi.html
  * サンプルデータは国土地理院提供のデータをそのままをホストしています。
* 自然災害伝承碑の画像は、[地理院地図の実装](https://github.com/gsi-cyberjapan/gsimaps)を参考に表示しています。

* MapLibre GL JS https://github.com/maplibre/maplibre-gl-js
  * https://maplibre.org/maplibre-gl-js-docs/example/cluster/
  * https://maplibre.org/maplibre-gl-js-docs/example/heatmap-layer/
* 国土地理院最適化ベクトルタイル https://github.com/gsi-cyberjapan/optimal_bvmap
