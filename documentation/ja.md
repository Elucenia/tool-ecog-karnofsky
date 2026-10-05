<!-- ELUCENIA technical documentation · ecog-karnofsky · ja · no clinical/professional/rights approval -->

# ECOG・Karnofsky

[条件・出典・許諾](https://elucenia.org/ja/tools/ecog-karnofsky)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### Karnofskyスケール

`kps`

- `0` — 0% · 死亡
- `10` — 10% · 瀕死
- `20` — 20% · 極めて重篤、積極的な支持療法が必要
- `30` — 30% · 重度の機能障害、入院が必要
- `40` — 40% · 機能障害があり、特別な介護が必要
- `50` — 50% · かなりの介助と頻回の医療ケアが必要
- `60` — 60% · 時々介助が必要
- `70` — 70% · 身の回りのことはできるが就労できない
- `80` — 80% · 努力を要するが通常の活動が可能
- `90` — 90% · 通常の活動が可能、症状・徴候はわずか
- `100` — 100% · 正常，症状や疾患の所見なし

## 方法の版

ECOG 0–5/Oken 1982、ECOG-ACRINのKPS対応90–100/70–80/50–60/30–40/10–20/0

## 記載された計算式

ECOG-ACRINの対応：Karnofsky 100–90% = ECOG 0、80–70% = ECOG 1、60–50% = ECOG 2、40–30% = ECOG 3、20–10% = ECOG 4、0% = ECOG 5（死亡）。

両尺度は同一ではありません。ECOG-ACRIN自身もこの表を対応づけの「一つの方法」としています。

## 限界・対象集団

ECOG-ACRINの表は、ECOGとKarnofskyの間で一般的に用いられる対応関係を示しており、尺度間を対応させる複数の方法の一つです。両尺度は機能的能力を記述し、試験の対象集団を定める助けとなります。換算だけでは治療の適格性は決まりません。機能評価と臨床プロトコルの基準を維持する必要があります。

## 参考文献

- [Oken MM et al. Toxicity and response criteria of the Eastern Cooperative Oncology Group. Am J Clin Oncol, 1982.](https://doi.org/10.1097/00000421-198212000-00014)

- [ECOG-ACRIN Cancer Research Group. ECOG Performance Status Scale (comparação com a escala de Karnofsky).](https://ecog-acrin.org/resources/ecog-performance-status/)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026
