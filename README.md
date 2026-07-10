# RAIN//LINE IKB — 池袋ナイトラン

雨の池袋を舞台にした、iPhoneブラウザ対応の短編オープンワールド風アクションゲームです。

プレイヤーは徒歩で街を探索し、車両に乗り換え、追跡を振り切って都市回線の復旧データを届けます。実在ブランドや既存ゲームの固有表現は使わず、架空の人物・団体・店舗で構成しています。

## 内容

- Canvasベースの2.5Dゲーム画面
- iPhone向けタッチ操作
  - 左スティック
  - アクションボタン
  - ダッシュ / ブレーキ
- 徒歩移動、車両操作、追跡、会話、ミッション進行
- 雨、ネオン、群衆、交通、池袋らしい高密度な街並み
- 専用生成アセット
  - タイトル背景
  - 主人公スプライト
  - 車両スプライト
  - 会話ポートレート
  - OGP画像

## 必要環境

- Node.js `>=22.13.0`

## 開発

```bash
npm install
npm run dev
```

このプロジェクトは Vinext / React 構成です。ローカル環境によっては Cloudflare Workers ランタイムの制約で `npm run dev` が動かない場合があります。その場合でも、以下でビルドと検証はできます。

```bash
npm test
npm run lint
```

## 検証

```bash
npm run typecheck
npm run test:unit
npm run build
npm run test:render
npm run lint
```

## 公開について

通常のGitHub Pagesは静的HTML配信のため、このVinextアプリをそのままサーバー実行する用途には向きません。公開する場合は、Sites / Cloudflare Workers互換のホスティングを推奨します。
