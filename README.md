# RAIN//LINE IKB — 池袋ナイトラン

雨の池袋を舞台にした、iPhoneブラウザ対応の短編オープンワールド風アクションゲームです。

このリポジトリには、GitHub Pagesでそのまま動く単体HTML版を配置しています。

## プレイ

- `index.html` がゲーム本体です。
- iPhone Safari / Chrome のブラウザで動作するよう、Canvas・タッチ操作・セーフエリア対応で構成しています。
- GitHub Pages が有効になると、以下のURLで公開されます。

```text
https://poinkare-kota.github.io/rainline-ikebukuro/
```

## 操作

- 左スティック: 移動
- ACTION: 車に乗る / 会話 / 回収
- DASH / BRAKE: 徒歩ではダッシュ、車ではブレーキ

## 内容

- 雨の池袋をモチーフにした架空のナイトシティ
- 徒歩移動、車両操作、追跡、会話、ミッション進行
- ネオン、雨、群衆、交通、警戒度、目的地マーカー
- 依存関係なし。`index.html` だけで動作

## GitHub Pages

`.github/workflows/pages.yml` を追加済みです。GitHub側で Pages が Actions デプロイに設定されていれば、`main` へのpush後に自動公開されます。

もし公開URLが出ない場合は、GitHubのリポジトリ画面で以下を確認してください。

1. `Settings` → `Pages`
2. `Build and deployment` の Source を `GitHub Actions` にする
3. `Actions` タブで `Deploy GitHub Pages` を手動実行、または次のpushを待つ

## 注意

実在ブランドや既存ゲームの固有表現は使わず、架空の人物・団体・店舗で構成しています。
