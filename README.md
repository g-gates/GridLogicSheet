# GridLogicSheet α — 配布

Linux（x86_64）向けの VBA マクロ検証ツールです。  
Excel の代替ではありません。α版として無償提供しています。

## ダウンロード

**最新版:** [Releases](https://github.com/g-gates/GridLogicSheet/releases) から ZIP を取得してください。

| 版 | ファイル |
|----|----------|
| 2026.06.08 | `GridLogicSheet-2026.06.08.zip` |

### SHA256

```
ZIP:
3b7de205ead2d62fe02bf039cb693fa0e820001548f108874cc1d88d507bb9e5

AppImage（ZIP 展開後の GridLogicSheet-2026.06.08/ 内）:
087a6a9cc4bcb29a7f6f81ec638e4e849cf73f466691ed0f1e8dee7f09918342
```

## 使い方（最短）

1. ZIP を展開する  
2. 展開フォルダで `bash run-gridlogic.sh` を実行する  
3. 「マクロ関連 ▼」から `AuditMacros` 内の `.bas` を読み込み、実行して確認する  

詳細は ZIP 内の `README.txt` と `Docs/` を参照してください。

## サポート範囲

- 同梱マクロ **01〜23** の実行結果の目視確認  
- `.xlsx` の新規・開く・保存（値・数式）  

サポートしない例: Windows / macOS、Linux 環境構築、Excel 完全互換、マクロの書き方代行。

## 既知の制限（α）

- ファイル保存時、セルの書式（背景色・文字色・太字など）は保存されません  
- 読み込んだ VBA マクロはブックに保存されません  

## 利用条件

利用条件・免責の全文は ZIP 内の `EULA.txt` が正本です。  
再配布・逆コンパイル等は EULA の禁止事項に従ってください。

## 言語について

- **初回配布（2026.06.08）:** 同梱ドキュメント・本 README・Release 説明は **日本語** です。
- **英語版:** 日本語版の配布と動作確認が一段落したあと、README / Release 説明 / 同梱 Docs の英語版を **別途追加予定** です（同時リリースではありません）。

**Language:** This first α release is documented in **Japanese**. An **English README and release notes** will be added later, after the Japanese distribution is verified. The downloadable ZIP is the same binary.

## 開発記・お知らせ

https://note.com/lc_gate_grid/n/n871a3ba155a9

**このリポジトリには配布物のみを置いています。ソースコードは公開していません。**
