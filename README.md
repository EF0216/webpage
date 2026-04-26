# README.md

## 概要

このリポジトリは、商品LPをHTML/CSSで作成し、GitHub Pagesで公開するためのリポジトリです。

主な目的は、商品企画・売場提案・商談用に使えるLPを素早く作成し、URLで共有できる状態にすることです。

## 公開ページ

トップ一覧ページ：

```text
https://ユーザー名.github.io/webpage/
```

各LP：

```text
https://ユーザー名.github.io/webpage/RIRALEGI-AW/
https://ユーザー名.github.io/webpage/RIRALEGI-SS/
```

## 基本構成

```text
webpage
├─ index.html
├─ AGENTS.md
├─ DESIGN_RULES.md
├─ README.md
├─ RIRALEGI-AW
│  ├─ index.html
│  └─ assets
└─ RIRALEGI-SS
   ├─ index.html
   └─ assets
```

## 各ファイルの役割

### index.html

トップのLP一覧ページです。

公開中のLPや今後追加するLPへのリンクを管理します。

### AGENTS.md

Codex / Claude Code などのAIエージェントに向けた作業ルールです。

### DESIGN_RULES.md

LPのデザイン方針・色・余白・画像・構成ルールをまとめたファイルです。

### 各LPフォルダ

商品・シーズン別のLPです。

例：

```text
RIRALEGI-AW
RIRALEGI-SS
```

各フォルダの中に `index.html` と `assets` を置きます。

## 画像管理

画像は各LPフォルダ内の `assets` に入れます。

例：

```text
RIRALEGI-AW/assets/hero.png
RIRALEGI-AW/assets/scene_aw.png
```

HTMLでは相対パスで呼び出します。

```html
<img src="assets/hero.png" alt="着用イメージ">
```

## 新しいLPの追加方法

1. 新しいフォルダを作る
2. フォルダ内に `index.html` と `assets` を入れる
3. 画像を `assets` に入れる
4. トップの `index.html` にリンクカードを追加する
5. GitHubにアップロードする
6. GitHub Pagesで表示確認する

例：

```text
webpage
├─ CHARACTER-SOCKS
│  ├─ index.html
│  └─ assets
```

URL：

```text
https://ユーザー名.github.io/webpage/CHARACTER-SOCKS/
```

## 修正時の注意

- 画像パスを壊さない
- フォルダ名を勝手に変えない
- 商品LPのデザインを大きく崩さない
- 画像は必ず `assets` に入れる
- ローカルPCの絶対パスを使わない
- スマホ表示も確認する

## GitHub Pages設定

GitHub Pagesは以下の設定を推奨します。

```text
Source: Deploy from a branch
Branch: main
Folder: /(root)
```

## 更新後の確認

更新後は、以下を確認します。

- トップ一覧ページが表示される
- 各LPページが表示される
- 画像がすべて表示される
- リンクが正しい
- PCで崩れていない
- スマホでも大きく崩れていない

## 運用方針

このリポジトリでは、複雑なWebシステム化よりも、商品LPを素早く作り、修正しやすく、URLで共有できることを優先します。

HTML/CSSはできるだけシンプルに保ち、今後の商品追加に対応しやすい形で管理します。
