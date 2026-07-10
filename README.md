# RAIN//LINE IKB — 池袋ナイトラン 3D

雨の池袋を舞台にした、iPhoneブラウザ対応の3Dオープンワールド風アクションゲームです。

このリポジトリには、GitHub Pagesでそのまま動く単体HTML版を配置しています。現在の版はWebGL/Three.jsによる3D版です。

## プレイ

- `index.html` がゲーム本体です。
- iPhone Safari / Chrome のブラウザで動作するよう、WebGL・タッチ操作・セーフエリア対応で構成しています。
- GitHub Pages が有効になると、以下のURLで公開されます。

```text
https://poinkare-kota.github.io/rainline-ikebukuro/
```

## 操作

- 左スティック: 移動
- ACTION: 車に乗る / 降りる / 回収
- RUN / BRAKE: 徒歩ではダッシュ、車ではブレーキ

## 内容

- 3Dの池袋風ナイトシティ
- 徒歩移動、車両操作、警備車両の追跡、会話、ミッション進行
- 雨、霧、ネオン看板、窓明かり、道路、群衆、交通、警戒度
- 建物・道路・車両・人物・照明をコードで生成
- 有料グラフィック素材なし

## 現実的な制約

iPhoneブラウザで動かすため、商用GTA級のフォトリアルモデルや巨大テクスチャは使っていません。現状は「軽量な3Dゲームプロトタイプ」です。写真のような品質に近づけるには、以下が必要です。

- 高品質な人物・車両・街区モデル
- PBRテクスチャ、法線マップ、反射マップ
- LoD、圧縮テクスチャ、アセットストリーミング
- iPhone向けの描画負荷最適化

このリポジトリでは、まずブラウザで確実に動く3D版を優先しています。

## GitHub Pages

`.github/workflows/pages.yml` を追加済みです。GitHub側で Pages が Actions デプロイに設定されていれば、`main` へのpush後に自動公開されます。

もし公開URLが出ない場合は、GitHubのリポジトリ画面で以下を確認してください。

1. `Settings` → `Pages`
2. `Build and deployment` の Source を `GitHub Actions` にする
3. `Actions` タブで `Deploy GitHub Pages` を手動実行、または次のpushを待つ

## 注意

実在ブランドや既存ゲームの固有表現は使わず、架空の人物・団体・店舗で構成しています。
