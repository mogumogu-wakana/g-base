# Copilot Instructions for g-base

## プロジェクト概要
- このリポジトリは、名古屋駅近くの大人向けeスポーツBAR「G-BASE」の静的Webサイトです。
- 主な構成は `index.html`、`css/style.scss`（Sassで管理）、`img/` ディレクトリの画像群です。
- JavaScriptやビルドツールは現状未使用。HTML/CSS/画像のみで構成。

## ディレクトリ構成
- `index.html` : サイトのメインページ。全セクション（CONCEPT, GAME, MENU, ACCESSなど）を1ページで管理。
- `css/style.scss` : サイト全体のスタイル。Sass変数・mixin・レスポンシブ設計あり。
- `css/style.css` : SassからビルドされたCSS。直接編集しない。
- `img/` : サイトで使用する画像（ロゴ、メニュー、アイコン等）。

## 開発・運用ワークフロー
- スタイル修正は `css/style.scss` を編集し、`style.css` へSassビルドする（例: `sass css/style.scss css/style.css`）。
- 画像追加時は `img/` 配下に配置し、HTML/CSSで参照。
- HTMLの構造変更は `index.html` のみで完結。
- JavaScript追加やビルドツール導入は未実施。必要時は新規導入方針を要確認。

## コーディング規約・パターン
- フォントやカラーはSass変数で一元管理。
- レイアウトや装飾はSassのmixin（例: `split-border-rectangle`）で共通化。
- レスポンシブ対応はSassのメディアクエリで管理。
- 画像パスは相対パスで指定。
- クラス命名はBEM未採用、シンプルな英語名。

## 参考ファイル
- `css/style.scss` : 変数・mixin・レスポンシブ設計例
- `index.html` : セクション構造、画像参照例

## 注意事項
- `style.css` はSassから自動生成されるため直接編集しない。
- JavaScriptや外部ライブラリ導入時は、既存構成との整合性に注意。
- 画像ファイル名・パスのtypoに注意。

---

AIエージェントは、上記方針・構成を遵守し、静的Webサイトとしての一貫性を保つようにしてください。
