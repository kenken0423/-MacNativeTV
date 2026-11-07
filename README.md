# MacNativeTV

MacNativeTVは、macOS上でEDCB・Amatsukaze・KonomiTVと対応チューナーを連携させる、非公式の実験的な統合パッケージです。各上流プロジェクトがMacNativeTVを公式にサポートしているわけではありません。

> **状態：2026年11月7日版の配布候補。現在、このGitHubリポジトリは非公開で、ダウンロード用リリースもまだ公開されていません。** 別のMacでの初回インストールや長時間録画は未確認です。安定動作を保証する製品ではありません。

## ダウンロード

リリース公開後、「Releases」から次の2ファイルをダウンロードしてください。

- `MacNativeTV-macOS-Intel-AppleSilicon-2026-11-07-license-reviewed.tar.gz`
- 同名の `.sha256` ファイル

展開する前に、ターミナルで次を実行してチェックサムが `OK` になることを確認します。

```sh
shasum -a 256 -c MacNativeTV-macOS-Intel-AppleSilicon-2026-11-07-license-reviewed.tar.gz.sha256
```

展開後は、アーカイブ内の `MacNativeTV/README.md` と `MacNativeTV/docs/配布利用ガイド.md` に沿って初回準備を行ってください。初回準備にはインターネット接続が必要です。チューナーのファームウェア本体はアーカイブに含めず、初期化時に指定済みの上流ソースから取得してハッシュを確認します。

## 必要なもの

- macOS 15以降のIntel MacまたはApple Silicon Mac
- DTV02A-5TS-PまたはPLEX PX-MLT5PEチューナーと、対応する給電ケース・アンテナ設備
- 暗号化放送を視聴する場合は、正規のB-CASカードと視聴契約
- 初回準備時に使えるインターネット接続

## ご利用前に

- まず短い試験録画を行い、大切な録画は別の場所にもバックアップしてください。
- 長時間録画、スリープ復帰、全チューナー・全チャンネルの動作は確認できていません。
- KonomiTVはChromeでの利用を推奨します。ブラウザーや画質によって再生状況が異なる場合があります。
- EDCBやKonomiTVのポートをインターネットへ直接公開しないでください。
- macOSのアプリはAppleの公証を受けていません。警告が出た場合も、Gatekeeper全体を無効にしないでください。
- 各部品のライセンスは異なります。再配布前に同梱の `THIRD_PARTY_NOTICES.md`、ライセンス文書、ソースを確認してください。特にEDCBの同梱条件では、商用・シェアウェアへの組み込みに許可が必要です。

## 上流プロジェクト

- [EDCB](https://github.com/xtne6f/EDCB)
- [Amatsukaze](https://github.com/nekopanda/Amatsukaze)
- [KonomiTV](https://github.com/tsukumijima/KonomiTV)
- [px4_drv](https://github.com/tsukumijima/px4_drv)
