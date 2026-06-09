# GridLogicSheet α — 配布

Linux（x86_64）向けの VBA マクロ検証ツールです。  
Excel の代替ではありません。α版として無償提供しています。

## ダウンロード

**最新版:** [Releases](https://github.com/g-gates/GridLogicSheet/releases) から ZIP を取得してください。

| 版 | ファイル | 内容 |
|----|----------|------|
| 2026.06.08 | [`GridLogicSheet-2026.06.08.zip`](https://github.com/g-gates/GridLogicSheet/releases/download/2026.06.08/GridLogicSheet-2026.06.08.zip) | アプリ本体（AppImage）+ 日本語 README / Docs |
| 2026.06.08 | [`GridLogicSheet-2026.06.08-docs-en.zip`](https://github.com/g-gates/GridLogicSheet/releases/download/2026.06.08/GridLogicSheet-2026.06.08-docs-en.zip) | **英語ドキュメントのみ**（アプリ本体は上記と同一バイナリ） |

### SHA256

```
アプリ ZIP (GridLogicSheet-2026.06.08.zip):
3b7de205ead2d62fe02bf039cb693fa0e820001548f108874cc1d88d507bb9e5

AppImage（ZIP 展開後の GridLogicSheet-2026.06.08/ 内）:
087a6a9cc4bcb29a7f6f81ec638e4e849cf73f466691ed0f1e8dee7f09918342

英語ドキュメント ZIP (GridLogicSheet-2026.06.08-docs-en.zip):
9ca7fd8d9c79e8d411416b5c17d9ac4d85546c85b14d2b6f4931eca78d7a7510
```

## 使い方（最短）

1. **`GridLogicSheet-2026.06.08.zip`** を展開する  
2. 展開フォルダで `bash run-gridlogic.sh` を実行する  
3. 「マクロ関連 ▼」から `AuditMacros` 内の `.bas` を読み込み、実行して確認する  

詳細は ZIP 内の `README.txt` と `Docs/`（日本語）を参照してください。  
英語の説明は **`GridLogicSheet-2026.06.08-docs-en.zip`** を展開した `README_EN.txt` と `Docs/*_EN.md` を参照してください。

## サポート範囲

- 同梱マクロ **01〜23** の実行結果の目視確認  
- `.xlsx` の新規・開く・保存（値・数式）  

サポートしない例: Windows / macOS、Linux 環境構築、Excel 完全互換、マクロの書き方代行。

## 既知の制限（α）

- ファイル保存時、セルの書式（背景色・文字色・太字など）は保存されません  
- 読み込んだ VBA マクロはブックに保存されません  
- **UI の英語化は一部のみ**（OS ロケールが `ja` 始まりなら日本語、それ以外は英語 UI になるが、一部文字列は日本語のまま）。詳細は英語ドキュメント内 `KNOWN_ISSUES_EN.md`

## 利用条件

利用条件・免責の全文は **アプリ ZIP 内** の `EULA.txt` が正本です（日本語）。  
再配布・逆コンパイル等は EULA の禁止事項に従ってください。

## 言語について

- **アプリ本体（2026.06.08）:** `GridLogicSheet-2026.06.08.zip` 内の README・Docs・EULA は **日本語** です。  
- **英語:** `GridLogicSheet-2026.06.08-docs-en.zip` に **英語ドキュメントのみ** を同梱しています。アプリの実行には **アプリ ZIP** が必要です。  
- **UI:** 英語ドキュメントの配布は、**アプリ UI の完全英語化ではありません**。  

## 開発記・お知らせ

- Note: https://note.com/lc_gate_grid/n/n871a3ba155a9

---

## English (documentation only)

This section describes **English documentation** for release `2026.06.08`.  
It is **not** a separate English application build.

### Download

**Releases:** https://github.com/g-gates/GridLogicSheet/releases

| Version | File | Contents |
|---------|------|----------|
| 2026.06.08 | [`GridLogicSheet-2026.06.08.zip`](https://github.com/g-gates/GridLogicSheet/releases/download/2026.06.08/GridLogicSheet-2026.06.08.zip) | Application (AppImage) + Japanese README / Docs |
| 2026.06.08 | [`GridLogicSheet-2026.06.08-docs-en.zip`](https://github.com/g-gates/GridLogicSheet/releases/download/2026.06.08/GridLogicSheet-2026.06.08-docs-en.zip) | **English documentation only** (same AppImage binary as above) |

### SHA256

```
Application ZIP (GridLogicSheet-2026.06.08.zip):
3b7de205ead2d62fe02bf039cb693fa0e820001548f108874cc1d88d507bb9e5

AppImage (inside GridLogicSheet-2026.06.08/ after extract):
087a6a9cc4bcb29a7f6f81ec638e4e849cf73f466691ed0f1e8dee7f09918342

English docs ZIP (GridLogicSheet-2026.06.08-docs-en.zip):
9ca7fd8d9c79e8d411416b5c17d9ac4d85546c85b14d2b6f4931eca78d7a7510
```

### Quick start

1. Download and extract **`GridLogicSheet-2026.06.08.zip`**  
2. Run `bash run-gridlogic.sh` in the extracted folder  
3. **Macro ▼** → import `.bas` from `AuditMacros/`, run, and verify on screen  

For English instructions, also extract **`GridLogicSheet-2026.06.08-docs-en.zip`** and read `README_EN.txt` and `Docs/*_EN.md`.

### Support scope

- Visual verification of bundled macros **01–23**  
- `.xlsx` New / Open / Save (values and formulas)  

Not supported: Windows / macOS, Linux environment setup, full Excel compatibility, writing macros for you.

### Known limitations (α)

- Cell formatting (colors, bold, etc.) is **not** saved to `.xlsx`  
- Imported VBA macros are **not** saved in the workbook  
- **UI localization is partial:** OS locale starting with `ja` → Japanese UI; otherwise English UI — but some strings remain Japanese. See `KNOWN_ISSUES_EN.md` in the docs-en pack.

### License

Authoritative license: `EULA.txt` inside the **application ZIP** (Japanese).  
No redistribution or reverse engineering per EULA.

### Language note

- **Application package:** Japanese README and Docs inside the main ZIP.  
- **English docs pack:** Documentation only — download `GridLogicSheet-2026.06.08-docs-en.zip`.  
- **Not** a full English UI release.

### Development log

- Note (Japanese): https://note.com/lc_gate_grid/n/n871a3ba155a9

---

**This repository contains distribution artifacts only. Source code is not published.**
