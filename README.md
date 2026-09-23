# Claude Code ハンズオン

Claude Code の基本操作からソフトウェア開発・チーム開発までを **全3 Section・計5.5時間**（Section 1 90分 / Section 2 120分 / Section 3 120分）で実践するハンズオンコースです。

題材には OSS の **[agmsg](https://github.com/fujibee/agmsg)**（CLI AI エージェント間のメッセージングツール。Bash + SQLite 製）を使い、ソースコード解析 → 機能追加 → レビュー → PR 作成 → チーム開発フローまでを一気通貫で体験します。

## 📖 教材の閲覧

ブラウザで [`index.html`](index.html)（コースポータル）を開くと、各 Section の資料にアクセスできます（外部依存なしの静的 HTML）。

```bash
open index.html
```

| ファイル | 内容 |
|---|---|
| [`index.html`](index.html) | コースポータル（概要・各 Section へのリンク） |
| [`session1.html`](session1.html) | Section 1：Claude Code の基本 |
| [`session2.html`](session2.html) | Section 2：Claude Code を使ったソフトウェア開発 |
| [`session3.html`](session3.html) | Section 3：Claude Code を使ったチーム開発 |
| [`HANDSON.md`](HANDSON.md) | 講義資料のソース（Markdown） |

## 🎯 学べること

- エージェントループ・コンテキスト・承認モードなど Claude Code の**基本の仕組みと操作**
- 既存 OSS リポジトリの**ソースコード解析**（構造把握 → 特定 → 深掘り → サマリ）
- CLAUDE.md / Skills / プラグイン / コネクタ / MCP / SubAgent / Hooks による**開発環境の整備と自動化**
- 機能追加 → AI レビュー → テスト生成 → PR 作成の**個人開発フロー**
- Issue 起点の開発フローとスキル化による**チーム開発の実践**
