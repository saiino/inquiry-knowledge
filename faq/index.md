# FAQ インデックス

Power Platform 問い合わせ対応のナレッジベース。
**Claude Code はまずこのファイルだけを読み、該当カテゴリのファイルのみを開くこと**(全件読み込み禁止。FAQが増えても検索コストを一定に保つため)。

## カテゴリ一覧

| カテゴリ | ファイル | 内容 | 件数 |
|---|---|---|---|
| Power BI / アプリ | [powerbi/apps.md](powerbi/apps.md) | アプリの公開・共有・閲覧権限・更新反映 | 2 |
| Power BI / ワークスペース | [powerbi/workspace.md](powerbi/workspace.md) | ワークスペースの権限・ロール・作成/削除 | 1 |
| Power BI / ライセンス | [powerbi/license.md](powerbi/license.md) | Pro/PPU/Fabric容量などライセンス関連 | 1 |
| Power BI / Fabric | [powerbi/fabric.md](powerbi/fabric.md) | Fabric容量・OneLake・Fabric固有機能 | 0 |
| Power Apps | [powerapps/general.md](powerapps/general.md) | キャンバスアプリ・モデル駆動型アプリ全般 | 0 |
| Copilot Studio | [copilotstudio/general.md](copilotstudio/general.md) | エージェント作成・公開・チャネル連携 | 0 |

## FAQ ID の規則

`FAQ-<カテゴリ略号>-<連番3桁>` 形式。略号は以下。

| 略号 | カテゴリ |
|---|---|
| PBI-APP | Power BI / アプリ |
| PBI-WS | Power BI / ワークスペース |
| PBI-LIC | Power BI / ライセンス |
| PBI-FAB | Power BI / Fabric |
| PA | Power Apps |
| CS | Copilot Studio |

連番はカテゴリごとに採番し、欠番が出ても詰めない(過去の回答メールに書いたIDが無効になるため)。

## 運用メモ

- FAQ の追加・更新は必ず PR 経由で行い、保守担当がレビューしてから merge する
- どのカテゴリにも当てはまらない問い合わせが増えてきたら、新カテゴリのファイルを作り、この表と略号表に行を追加する
- 件数列は FAQ 追加 PR の中で一緒に更新する
- 各エントリは `種別`(Microsoft仕様 / 社内運用)と `最終確認日` を持つ。`Microsoft仕様` のエントリは faq-reviewer スキルで**月1回を目安に棚卸し**する(Microsoft Learn の現行記述と突き合わせ、古くなった記述を修正PR化)。`社内運用` は棚卸し対象外
