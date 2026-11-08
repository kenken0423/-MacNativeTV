# 同梱ソフトウェアのライセンス・ソース・ファームウェアについて

更新日：2026年11月9日

MacNativeTVは複数の独立したソフトウェアを組み合わせた非公式のmacOS向けパッケージです。パッケージ全体に単一のライセンスが適用されるわけではありません。以下は主要部品の概要であり、各ライセンス本文に代わるものではありません。個別の配布条件はアーカイブ内の原文を確認してください。

| 部品 | 主な条件 | 同梱ソース・ライセンス資料 |
|---|---|---|
| MacNativeTV受信機・px4_drv由来コード | GPL-2.0-only | `LICENSE`、`receiver/licenses/`、`receiver/source/`、`receiver-native/` |
| EDCB | 同梱READMEはフリーソフトへの改変・組み込みと公開時のソース添付を記載する一方、商用・シェアウェアへの組み込みには許可が必要と記載 | `edcb/licenses/EDCB-Readme.txt`、`edcb/licenses/`、`edcb/source/`、`edcb/patches/` |
| Amatsukaze | 上流READMEによるとGPLライブラリを含み、プログラム全体にGPLが適用。依存部品には個別条件も適用 | `amatsukaze/licenses/`、`amatsukaze/source/`、`versions.json`、ランタイムの通知 |
| KonomiTV | 上流本体はMIT。MacNativeTV独自改修を含む | `konomitv/source/`、`konomitv/licenses/` |
| KonomiTV用FFmpeg | x264・x265を有効化したGPL構成 | FFmpeg/x265/x264ソース、`konomitv/build-media.sh` |
| B25補助プロセス、CivetWeb、Lua、ランタイム等 | Apache-2.0、MIT、その他。部品ごとに異なる | `decoder/`、`edcb/licenses/`、各ランタイム・依存の通知ファイル |

配布アーカイブには主要な対応ソーススナップショット、適用パッチ、取得元・版を示す情報、ビルド設定、ライセンス原文を収録しています。細かな依存パッケージの条件も各通知ファイルで確認してください。

## ファームウェア

チューナー初期化用の `it930x-firmware.bin` はアーカイブに含めていません。対象ファームウェアの再配布権を明確に示すライセンスを確認できなかったためです。初回初期化時、利用者のMacから固定した上流ソースを取得し、SHA-256を検証します。この方法でファームウェアの再配布権を主張するものではありません。

- 上流：`tsukumijima/px4_drv`
- 固定コミット：`6238187cbd2f334aec55d078fe58eaac7c255125`
- SHA-256：`5213a5a38872661277a2cc1b2dfdfe88faf06f41205f460f3b51857f0568b484`

## 上流プロジェクト

- [EDCB](https://github.com/xtne6f/EDCB)
- [Amatsukaze](https://github.com/nekopanda/Amatsukaze)
- [KonomiTV](https://github.com/tsukumijima/KonomiTV)
- [px4_drv](https://github.com/tsukumijima/px4_drv)

これは条件の日本語要約であり、法律相談ではありません。特にEDCBの条件上、本版は無償の実験版として配布します。有料提供や商用利用を検討する場合は、事前に権利者へ確認してください。
