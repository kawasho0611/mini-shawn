# コントリビューションガイド

このドキュメントへの貢献に興味を持っていただきありがとうございます！  
以下のガイドラインに沿って、Pull Request や Issue を作成してください。

## 💡 貢献の種類

| 種類 | 説明 |
|------|------|
| 🐛 修正 | 誤字脱字、リンク切れ、事実誤認の修正 |
| ✨ 改善 | 既存コンテンツの加筆・表現改善 |
| 📝 新規 | 新しいページやセクションの追加提案 |
| 💬 質問 | 内容への質問や不明点 → Issue で |

## 🔧 Pull Request の手順

### 1. フォークとクローン

```bash
# リポジトリをフォーク（GitHub上で）
git clone https://github.com/YOUR_USERNAME/mini-shawn.git
cd mini-shawn
git remote add upstream https://github.com/kawasho0611/mini-shawn.git
```

### 2. ブランチを作成

```bash
git checkout -b fix/typo-in-flow  # 例：選考フローの誤字修正
```

**ブランチ命名規則:**

- `fix/` … 修正
- `improve/` … 改善
- `add/` … 新規追加
- `docs/` … ドキュメント構成の変更

### 3. ローカルで確認

```bash
pip install -r requirements.txt
mkdocs serve
# http://localhost:8000 で表示を確認
```

### 4. コミット＆プッシュ

```bash
git add .
git commit -m "fix: 選考フローページの誤字を修正"
git push origin fix/typo-in-flow
```

**コミットメッセージ規則:**

- `fix:` 修正
- `improve:` 改善
- `add:` 新規追加
- `chore:` 設定変更など

### 5. Pull Request を作成

GitHub上でPull Requestを作成してください。テンプレートが表示されるので、内容を記入してください。

## 📏 コンテンツガイドライン

- **読者を意識する**: 採用候補者、社外の方が読むことを前提に書いてください
- **やさしい日本語**: 専門用語には説明を添え、平易な表現を心がけてください
- **事実ベース**: 主観的な表現よりも、具体的な事実やデータを優先してください
- **画像**: `docs/assets/` フォルダに配置してください

## ⚖️ レビュープロセス

1. PR作成後、メンテナーが **3営業日以内** にレビューします
2. 修正依頼がある場合はコメントでお知らせします
3. 承認後、メンテナーがマージします

## 🙏 行動規範

- 建設的で丁寧なコミュニケーションを心がけてください
- すべての貢献者を尊重してください
- 不適切な内容や攻撃的な表現は受け入れません
