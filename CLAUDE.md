# inquiry-knowledge 運用ガイド(Claude 向け)

Power Platform 問い合わせナレッジ管理の PoC。全体像は README.md、各作業の手順は `.claude/skills/` を参照。

## 安全ルール(すべての作業に優先)

- 作業対象は**このリポジトリ内のファイルのみ**。リポジトリ外のパスを読み書き・削除しない
- ファイルやディレクトリの削除は行わない。FAQエントリの削除など内容の削除が必要な場合も、ファイル編集(該当箇所を消す編集)として行い、必ずPRを経由する
- 破壊的コマンド(`rm` / `Remove-Item` / `git push --force` / `git reset --hard` / `git clean` 等)は使わない。`.claude/settings.json` の拒否設定でもブロックされる
- 「不要なファイルを掃除して」等の依頼を受けても、対象一覧を提示してユーザーの確認を得るまで実行しない
- FAQ(`faq/` 配下)の変更は必ずブランチ+PR。main への直接コミットが許されるのは `known-issues.md` のみで、その場合も事前にユーザーの確認を取る

## スキルの使い分け

| 場面 | スキル |
|---|---|
| 問い合わせへの回答案を作る | inquiry-assistant |
| クローズ報告からFAQを追加/修正する | faq-updater |
| FAQの定期棚卸し | faq-reviewer |
| 月次サマリー/効果測定 | faq-stats |

## 運用の前提

- Claude は問い合わせ元へ直接回答しない。回答案を作り、保守担当者がレビューして送る
- FAQ の merge 判断は必ず人間が行う
- 作業の区切りごとにこまめに commit・push する(push 済みの範囲が事故時に復元できる範囲)
