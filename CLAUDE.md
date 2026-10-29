# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## リポジトリ概要

Claude Code ハンズオン（全3 Section・計5.5時間。Section 1 90分 / Section 2 120分 / Section 3 120分）の教材リポジトリ。ビルド・テスト・依存パッケージは無く、静的 HTML と Markdown のみで構成される。閲覧確認は `open index.html`。

## ファイル構成と編集ルール

- `HANDSON.md` — 講義資料のソース（Markdown）。**内容の変更はまずここに行う**
- `session1.html` 〜 `session3.html` — 各 Section の講義資料（HANDSON.md から手動で HTML 化したもの）。**HANDSON.md を変更したら、対応する session*.html にも必ず同じ変更を反映する**
- `session1-app.html` — Section 1 のデスクトップアプリ版（session1.html の変更を手動で反映する）
- `backlog-md.html` — Backlog.md を GitHub Codespaces で動かす手順（スクリーンショットは `Image/backlog-md/`）
- `index.html` — コースポータル（概要・各 Section へのカード型リンク）
- `Image/` — スクリーンショット・図版置き場。ファイル名は ASCII セーフ（例: `status.png`, `issue-flow.svg`）を維持する

## スタイル・表記

- 全 HTML は外部依存なしの単一ファイル。CSS は各ファイルに同一のものを埋め込んであり、デザイントークン（アンバー基調 `--accent: #d97706`、`.callout` / `.prompt-box` / `.lesson` 等のコンポーネント）を共有する。新ページを作る場合は既存ページの CSS をコピーして使う
- 日本語テキストは Unicode **NFC** で統一する（過去に NFD（濁点分離）混入で Edit の文字列一致が失敗した経緯あり）
- 各 Section の時間配分は所定の合計（Section 1 90分 / Section 2 120分 / Section 3 120分）に合わせる。セクションの分数を変更したら、その Section の合計に一致するよう再配分する
- コマンド例は題材（Backlog.md: TypeScript + Bun。ハンズオン用 fork は `cl-y-arai/Backlog.md-handson`）に合わせる（`bun run test`、`bun run check` 等）。実行環境は GitHub Codespaces、コードの修正はローカルの Claude Code、という前提で書く（ローカルでは Bun を動かさない）
