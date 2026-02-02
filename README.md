# Claude Code Skills Collection

Claude Code用のカスタムスキル集。

## スキル一覧

### create-study-material

OCR済みPDFから学習コンテンツ（キーワード解説・要約・理解確認問題）を自動生成するスキル。

**使用方法:**
```
/create-study-material <PDFパス>
```

**出力:**
- 各章のキーワード解説
- 内容要約
- 理解確認問題（記述式・○×問題・穴埋め問題）
- 総合問題

**依存関係:**
- Python 3.x
- PyMuPDF (`pip install pymupdf`)

## インストール方法

1. このリポジトリをクローン
2. `.claude/commands/` をプロジェクトの `.claude/commands/` にコピー
3. `scripts/extract_pdf_text.py` をプロジェクト内の適切な場所に配置し、スキルファイル内のパスを修正

```bash
git clone https://github.com/yourusername/for_sharing_skills.git
cp -r for_sharing_skills/.claude/commands/* ~/.claude/commands/
```

## ライセンス

MIT License
