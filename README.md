# MacNativeTV

MacNativeTVは、macOS上でEDCB・Amatsukaze・KonomiTVと対応チューナーを連携させる非公式の実験的な統合パッケージです。上流プロジェクトの公式製品ではなく、各開発者のサポート対象でもありません。

> **無償テスト版 v0.1.0-test.1**  
> 別のMacでの初回導入、長時間運転、全チューナー・全地域の動作は未確認です。安定した録画環境を保証しません。まず短い試験録画を行い、大切な録画をバックアップしてください。

## ダウンロード

[リリース一覧](https://github.com/kenken0423/-MacNativeTV/releases)から以下をダウンロードしてください。

- `MacNativeTV-v0.1.0-test.1-macOS-Intel-AppleSilicon.tar.gz`
- 同名の `.sha256` ファイル

展開前に、ターミナルでチェックサムを確認します。

```sh
shasum -a 256 -c MacNativeTV-v0.1.0-test.1-macOS-Intel-AppleSilicon.tar.gz.sha256
```

`OK`を確認してから展開し、アーカイブ内の日本語READMEと利用ガイドに沿って初回準備を行ってください。初回準備にはインターネット接続が必要です。

## 必要なもの

- macOS 15以降のIntel MacまたはApple Silicon Mac
- DTV02A-5TS-PまたはPLEX PX-MLT5PEチューナー、対応する給電ケース、アンテナ設備
- 暗号化放送には、正規のB-CASカードと視聴契約
- 初回準備時のインターネット接続

## 重要事項

- Appleの公証を受けていません。macOSの警告が出た場合もGatekeeper全体を無効にしないでください。
- ファームウェアは再配布条件を確認できなかったためアーカイブに含めません。初回準備時に固定した上流ソースから取得し、ハッシュを検証します。
- 各同梱部品は異なるライセンスに従います。アーカイブ内の `THIRD_PARTY_NOTICES.md`、各ライセンス原文、対応ソースを確認してください。EDCBの同梱説明では、商用・シェアウェアへの組み込みには許可が必要とされています。本版は無償配布です。
- EDCBやKonomiTVのポートをインターネットへ直接公開しないでください。KonomiTVはChromeを推奨します。

## 上流プロジェクト

- [EDCB](https://github.com/xtne6f/EDCB)
- [Amatsukaze](https://github.com/nekopanda/Amatsukaze)
- [KonomiTV](https://github.com/tsukumijima/KonomiTV)
- [px4_drv](https://github.com/tsukumijima/px4_drv)
