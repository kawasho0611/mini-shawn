# 📖 採用・組織ドキュメント

河上の採用プロセス、カルチャー、組織づくりについてのオープンドキュメントです。

## 🌐 サイトを見る

👉 [https://kawasho0611.github.io/mini-shawn/](https://kawasho0611.github.io/mini-shawn/)

## 🤝 コントリビューション

このドキュメントはオープンソースとして公開しており、どなたでも改善提案を出すことができます。

- 誤字脱字の修正、内容の改善提案 → **Pull Request** を送ってください
- 質問や提案 → **Issue** を作成してください

詳しくは [CONTRIBUTING.md](./CONTRIBUTING.md) をご覧ください。

## 🛠 ローカルで動かす

```bash
# リポジトリをクローン
git clone https://github.com/kawasho0611/mini-shawn.git
cd mini-shawn

# 依存パッケージをインストール
pip install -r requirements.txt

# ローカルサーバーを起動（http://localhost:8000 で確認）
mkdocs serve
```

## 📄 ライセンス

このドキュメントは [CC BY 4.0](./LICENSE) ライセンスの下で公開されています。

# mini-shawn

河上のこれまでの経験・知識・判断基準を言語化し、採用・組織・人事業務の企画/推進/運営を支援するための実験用リポジトリです。

このリポジトリは、Claude Code などの AI エージェントが参照・活用できるように、知識・判断ルール・テンプレート・実行ガイドを整理して公開していくことを目的としています。

## このリポジトリで目指すこと

- 採用・組織・人事に関する実務知見を再利用可能な形で整理する
- AI エージェントが参照しやすい構造で知識を蓄積する
- 他の人がインストールして、mini-shawn を業務支援エージェントとして使えるようにする
- ドキュメントの公開と、エージェント資産の管理を両立する

## 想定ユースケース

- 求人票の改善
- 採用戦略や採用計画の整理
- カジュアル面談/面接設計
- Value 設計や組織浸透施策の整理
- 採用オペレーションや定例運営の改善
- 人事・採用まわりの論点整理やたたき台作成

## 基本思想

mini-shawn は、単なるドキュメント置き場ではなく、以下の4層で構成することを想定しています。

1. `docs/` : 外部向けに読むための公開ドキュメント
2. `knowledge/` : 実務知見そのもの
3. `agents/` / `prompts/` : AI エージェントが動くための定義や指示
4. `evals/` : 出力品質を検証するための評価資産

## 推奨ディレクトリ構成

```text
mini-shawn/
├─ README.md
├─ LICENSE
├─ CONTRIBUTING.md
├─ mkdocs.yml
├─ docs/
│  ├─ index.md
│  ├─ concept/
│  ├─ install/
│  ├─ guides/
│  └─ examples/
├─ knowledge/
│  ├─ domains/
│  │  ├─ recruiting/
│  │  ├─ organization/
│  │  └─ operations/
│  ├─ playbooks/
│  ├─ heuristics/
│  ├─ templates/
│  └─ glossary/
├─ agents/
├─ prompts/
│  ├─ system/
│  ├─ tasks/
│  └─ routing/
├─ schemas/
├─ examples/
├─ evals/
├─ data/
├─ scripts/
└─ .github/
   └─ workflows/
```

## ディレクトリの役割

### `docs/`
公開サイト用のドキュメントです。導入方法、思想、利用例など、人が読むための情報を整理します。

### `knowledge/`
mini-shawn の中核です。採用・組織・人事に関する知見を蓄積します。

- `domains/` : 領域ごとの知識
- `playbooks/` : 実務の進め方
- `heuristics/` : 判断基準やレビュー観点
- `templates/` : 再利用可能なテンプレート
- `glossary/` : 用語集

### `agents/`
エージェントの役割定義を置く場所です。たとえば、採用戦略担当、面接設計担当、組織開発担当などを分けて定義します。

### `prompts/`
タスク実行用のプロンプト資産です。system prompt、task prompt、routing ルールなどを整理します。

### `schemas/`
入力・出力形式をそろえるための JSON Schema などを置きます。

### `examples/`
サンプル入力・サンプル出力・ケーススタディを置きます。

### `evals/`
出力品質を評価するための benchmark や rubric、期待出力例を管理します。

## まず最初に作るとよさそうなテーマ

### knowledge
- 採用戦略
- 求人票改善
- カジュアル面談設計
- 面接設計
- Value / 組織浸透

### templates
- 求人票テンプレート
- ヒアリングシート
- Value アンケート
- 採用定例アジェンダ
- 採用課題整理シート

### heuristics
- 何を優先して見るか
- 良いアウトプットの判断基準
- よくある失敗パターン
- 提案時に避けるべきこと

## ローカルでの使い方

```bash
# リポジトリをクローン
 git clone https://github.com/kawasho0611/mini-shawn.git
 cd mini-shawn

# 必要に応じて依存をインストール
pip install -r requirements.txt

# ドキュメントサイトをローカル起動
mkdocs serve
```

## 今後やりたいこと

- 知識ファイルのフォーマットを標準化する
- Claude Code 向けの agent / prompt 資産を整える
- 代表ユースケースごとのサンプルを増やす
- eval を整備して、mini-shawn の品質改善サイクルを回す

## 注意事項

このリポジトリに含まれる知識やテンプレートは、特定状況における判断支援を目的としたものです。実際の採用・組織・労務・法務判断にあたっては、必要に応じて専門家確認を行ってください。

## ライセンス

ライセンス方針は今後整理予定です。公開範囲・再利用条件に応じて更新します。
