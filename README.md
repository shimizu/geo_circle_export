# Geo Circle Export - 地理的円描画ツール

地図上に大圏円（球面上の円）を描画し、SVG/PNGとしてエクスポートできるWebアプリケーションです。

https://shimizu.github.io/geo_circle_export/

## 機能

- **大圏円の描画** — 地図をクリックして任意の地点に円を配置。半径はkm単位で指定可能
- **球面上の正確な計算** — 平面近似ではなく、地球を球体とみなした球面上で円を計算（`d3.geoCircle()`）
- **複数の投影法** — Natural Earth / メルカトル / 正射図法 / 正距円筒図法 / 方位等積図法 / 円錐等積図法
- **地図操作** — 左ドラッグで回転、右ドラッグで平行移動、ホイールでズーム
- **エクスポート** — SVG / PNG形式でダウンロード

## 技術スタック

- [D3.js](https://d3js.org/) — 地図投影・描画
- [d3-thematika](https://github.com/niccokunzmann/d3-thematika) — 地図レイヤー管理
- [Vite](https://vitejs.dev/) + Babel + Sass — ビルド環境

## セットアップ

```bash
git clone git@github.com:shimizu/geo_circle_export.git
cd geo_circle_export
npm install
```

## コマンド

```bash
npm run dev       # 開発サーバー起動
npm run build     # 本番ビルド（出力先: dist/）
npm run preview   # ビルド結果のプレビュー
npm run deploy    # GitHub Pages へデプロイ
```
