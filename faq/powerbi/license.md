# Power BI / ライセンス

Pro / PPU / Fabric容量などライセンスに関するFAQ。

---

## FAQ-PBI-LIC-001: レポートを開くと「Pro ライセンスが必要です」と表示される

- 登録日: 2026-07-16 / 更新日: 2026-07-16
- 種別: Microsoft仕様 / 最終確認日: 2026-07-17
- タグ: `Pro` `無料ライセンス` `容量`
- ステータス: サンプル(動作確認用。実案件のFAQ登録後に削除してよい)

### 症状 / 問い合わせ内容

共有されたレポートやアプリを開こうとすると、Pro ライセンスへのアップグレードを促される。

### 原因

コンテンツが共有容量(Pro ワークスペース)にあり、閲覧者側にも Pro ライセンスが必要な構成になっている。無料ライセンスで閲覧できるのは、Fabric 容量(F64 以上)または Premium 容量に配置されたコンテンツのみ。

### 解決方法

以下のいずれかで対応する。

1. 閲覧者に Pro ライセンスを割り当てる(少人数ならこちらが早い)
2. ワークスペースを F64 以上の Fabric 容量に割り当て、無料ライセンスでの閲覧を可能にする(全社向けなど閲覧者が多い場合)

どちらにするかはコスト比較になるため、閲覧者数を確認してから提案すること。

### 参考リンク

- [Power BI のライセンスの種類 - Microsoft Learn](https://learn.microsoft.com/ja-jp/power-bi/fundamentals/service-features-license-type)
- [Microsoft Fabric のライセンス - Microsoft Learn](https://learn.microsoft.com/ja-jp/fabric/enterprise/licenses)(F64未満はPro必須、F64以上でFree閲覧可の根拠)
