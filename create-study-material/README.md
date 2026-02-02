# create-study-material

OCR済みPDFから学習コンテンツ（キーワード解説・要約・理解確認問題）を自動生成するClaude Codeスキル。

## 使用方法

```
/create-study-material <PDFパス>
```

## 出力内容

各章ごとに以下を生成:
- 学習目標
- 前提知識
- 学習時間目安
- キーワード解説（5〜15個）
- 内容要約
- 理解確認問題（記述式・○×問題・穴埋め問題、解答・解説付き）

最後に章横断的な総合問題を生成。

## 出力ファイル

`{PDFファイル名}_study.md`（PDF同階層に生成）

## 依存関係

- Python 3.x
- PyMuPDF (`pip install pymupdf`)

## インストール

```bash
# スキルファイルをコピー
cp .claude/commands/create-study-material.md ~/.claude/commands/

# ヘルパースクリプトを配置（パスは適宜変更）
cp scripts/extract_pdf_text.py ~/Projects/OCR/
```

スキルファイル内の `extract_pdf_text.py` のパスを環境に合わせて修正してください。

## 対象

- 技術書、教科書など学習目的の書籍
- OCR済みPDF（テキストレイヤー付き）
