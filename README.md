# Claude Code Skills Collection

Claude Code用のカスタムスキル集。

## スキル一覧

### [create-study-material](./create-study-material/)

OCR済みPDFから学習コンテンツ（キーワード解説・要約・理解確認問題）を自動生成するスキル。

**使用方法:**
```
/create-study-material <PDFパス>
```

**詳細:** [create-study-material/README.md](./create-study-material/README.md)

## インストール方法

使いたいスキルのディレクトリから `.claude/commands/` をコピー:

```bash
git clone https://github.com/hirom-working/for_sharing_skills.git
cp -r for_sharing_skills/create-study-material/.claude/commands/* ~/.claude/commands/
```

## ライセンス

MIT License
