# GridLogicSheet α — 配布

Linux（x86_64）向けの VBA マクロ検証ツールです。  
Excel の代替ではありません。α版として無償提供しています。

## ダウンロード

**最新版:** [Releases](https://github.com/g-gates/GridLogicSheet/releases) から ZIP を取得してください。

| 版 | ファイル | 内容 |
|----|----------|------|
| **2026.06.23** | [`GridLogicSheet-2026.06.23.zip`](https://github.com/g-gates/GridLogicSheet/releases/download/2026.06.23/GridLogicSheet-2026.06.23.zip) | アプリ本体（AppImage）+ 日本語・英語 README / Docs + 監査マクロ **01〜28** |
| 2026.06.08 | [`GridLogicSheet-2026.06.08.zip`](https://github.com/g-gates/GridLogicSheet/releases/download/2026.06.08/GridLogicSheet-2026.06.08.zip) | 初回 α（日本語 Docs のみ・マクロ 01〜23） |
| 2026.06.08 | [`GridLogicSheet-2026.06.08-docs-en.zip`](https://github.com/g-gates/GridLogicSheet/releases/download/2026.06.08/GridLogicSheet-2026.06.08-docs-en.zip) | **英語ドキュメントのみ**（2026.06.08 バイナリ向け） |

### SHA256（2026.06.23）

```
アプリ ZIP (GridLogicSheet-2026.06.23.zip):
a0268bafcb18ca08d206d53971187a4455f3f584d4ebb84f93d7c44f12cbb53d

AppImage（ZIP 展開後の GridLogicSheet-2026.06.23/ 内）:
9c218e76e0802a5be3af6f3f644129e9d888a4fc5c4470f0459a7dd8f0129be6
```

## 使い方（最短）

1. **`GridLogicSheet-2026.06.23.zip`** を展開する  
2. 展開フォルダで `bash run-gridlogic.sh` を実行する  
3. 「マクロ関連 ▼」から `AuditMacros` 内の `.bas`（**01〜28**）を読み込み、実行して確認する  

詳細は ZIP 内の `README.txt`（日本語）と `README_EN.txt` / `Docs/*_EN.md`（英語）を参照してください。

## サポート範囲（2026.06.23）

- 同梱マクロ **01〜28** の実行結果の目視確認  
- `.xlsx` の新規・開く・保存（値・数式）  
- セル書式の一部保存（背景色・文字色・太字・斜体・下線・フォントサイズ）

サポートしない例: Windows / macOS、Linux 環境構築、Excel 完全互換、マクロの書き方代行。

## 既知の制限（α）

- **セル書式:** 背景色・文字色・太字・斜体・下線・フォントサイズは .xlsx 保存後、アプリ内で再 Open すると復元されます。**配置（ht）** など一部書式はまだ保存されません
- 読み込んだ VBA マクロはブックに保存されません
- **UI 言語:** GridLogic のメニュー・ステータス・About・ファイルダイアログは **日英対応**（OS が `ja` 始まりなら日本語、それ以外は英語）。FortuneSheet 組み込み UI や `run-gridlogic.sh` の一部メッセージは日本語のみの場合があります
- 数式バーの編集体感は Excel と一致しないことがあります（詳細は `KNOWN_ISSUES_JA.md`）

詳細は ZIP 内 `Docs/KNOWN_ISSUES_JA.md` / `KNOWN_ISSUES_EN.md`

## 利用条件

利用条件・免責の全文は **アプリ ZIP 内** の `EULA.txt` が正本です（日本語）。  
再配布・逆コンパイル等は EULA の禁止事項に従ってください。

## 言語について

- **2026.06.23 ZIP:** 日本語 README・Docs に加え、**同梱 ZIP 内** に英語 README・Docs があります。  
- **2026.06.08:** 英語は別 ZIP `GridLogicSheet-2026.06.08-docs-en.zip` を参照してください。  
- **UI:** GridLogic HUD は日英対応。FortuneSheet 組み込み UI 等は制限が残る場合があります（`KNOWN_ISSUES_JA.md` 参照）

## 開発記・お知らせ

- Note: https://note.com/lc_gate_grid

---

## English

Linux (x86_64) VBA macro verification tool. Not a replacement for Excel.

### Download

**Releases:** https://github.com/g-gates/GridLogicSheet/releases

| Version | File | Contents |
|---------|------|----------|
| **2026.06.23** | [`GridLogicSheet-2026.06.23.zip`](https://github.com/g-gates/GridLogicSheet/releases/download/2026.06.23/GridLogicSheet-2026.06.23.zip) | AppImage + JA/EN README and Docs + audit macros **01–28** |
| 2026.06.08 | [`GridLogicSheet-2026.06.08.zip`](https://github.com/g-gates/GridLogicSheet/releases/download/2026.06.08/GridLogicSheet-2026.06.08.zip) | First alpha (Japanese docs, macros 01–23) |
| 2026.06.08 | [`GridLogicSheet-2026.06.08-docs-en.zip`](https://github.com/g-gates/GridLogicSheet/releases/download/2026.06.08/GridLogicSheet-2026.06.08-docs-en.zip) | English docs only (2026.06.08 binary) |

### SHA256 (2026.06.23)

```
Application ZIP (GridLogicSheet-2026.06.23.zip):
a0268bafcb18ca08d206d53971187a4455f3f584d4ebb84f93d7c44f12cbb53d

AppImage (inside GridLogicSheet-2026.06.23/ after extract):
9c218e76e0802a5be3af6f3f644129e9d888a4fc5c4470f0459a7dd8f0129be6
```

### Quick start

1. Download and extract **`GridLogicSheet-2026.06.23.zip`**  
2. Run `bash run-gridlogic.sh` in the extracted folder  
3. **Macro ▼** → import `.bas` from `AuditMacros/` (01–28), run, and verify on screen  

Read `README_EN.txt` and `Docs/*_EN.md` inside the ZIP.

### Support scope (2026.06.23)

- Visual verification of bundled macros **01–28**  
- `.xlsx` New / Open / Save (values and formulas)  
- Partial cell format persistence (background, font color, bold, italic, underline, font size)

Not supported: Windows / macOS, Linux environment setup, full Excel compatibility, writing macros for you.

### Known limitations (α)

- **Cell formatting:** Background, font color, bold, italic, underline, and font size persist after SaveAs and in-app re-open. **Alignment (ht)** and some other formats are not saved yet
- Imported VBA macros are not saved in the workbook
- **UI language:** GridLogic menus, status bar, About, and file dialogs support **Japanese and English** (OS `ja*` → Japanese; otherwise English). FortuneSheet built-in UI and some `run-gridlogic.sh` messages may remain Japanese only
- Formula bar editing may not feel identical to Excel (see `KNOWN_ISSUES_EN.md`)

### License

Authoritative license: `EULA.txt` inside the application ZIP (Japanese).

### Development log

- Note (Japanese): https://note.com/lc_gate_grid

---

**This repository contains distribution artifacts only. Source code is not published.**
