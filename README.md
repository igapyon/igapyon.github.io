# igapyon.github.io

`igapyon` 個人サイト用の静的ファイルを置くリポジトリです。

現在の主な内容:

- `index.html`: サイトのトップページ
- `update-htmls.sh`: 配置先サーバーで HTML を取得して更新するためのスクリプト
- `apps/`: 個別アプリ用の配置ディレクトリ

## 概要

トップページはシンプルな静的 HTML で構成されており、日記、GitHub、Instagram などへのリンクをまとめています。

## 更新方法

### トップページを更新する場合

このリポジトリの `index.html` を編集して反映します。

### 配置先サーバーで更新する場合

`update-htmls.sh` は `/var/www/html` 配下で以下を更新する想定です。

- `index.html`
- `apps/klondike.html`
- `update-htmls.sh` 自身

取得元は GitHub 上の `devel` ブランチです。

## 補足

- 現在の `apps/` にはプレースホルダーとして `.gitkeep` のみがあります
- 実運用では `apps/klondike.html` を外部リポジトリから取得する前提になっています
