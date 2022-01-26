# QENTS：テキスト平易化の品質推定のためのデータセット [[English]](https://github.com/yu-hiro/qents/blob/main/README.en.md)

英語のテキスト平易化の品質推定のために、以下の特徴を持つデータセットを構築しました。

- Newselaコーパスの評価用データ1,077文に対する10種類のテキスト平易化システムの出力文を人手評価しました。
- 文法性、同義性、平易性、総合評価の4つの観点について、それぞれ4段階（1:最低、4:最高）でラベル付けしました。


## テキストとラベルの例

原文：Henson , who lived to age 93 , was born in southern Maryland .

||モデル|文法性|同義性|平易性|総合評価|
| :--- | :---: | :---: | :---: | :---: | :---: |
|Henson was born in Maryland and lived to be 93 years old .|Reference|4|3|3|4|
|Henson , who lived to age , for instance , was born in Maryland .|[PBMT-R](https://aclanthology.org/P12-1107)|1|1|1|1|
|henson lived was born .|[Hybrid](https://aclanthology.org/P14-1041)|1|1|1|1|
|Henson was born in southern Maryland .|[EncDecA](https://aclanthology.org/D15-1166)|4|3|4|3|
|Henson lived to age 93 .|[DRESS](https://aclanthology.org/D17-1062)|4|3|4|3|
|henson lived in maryland .|[S2S-All-FA](https://aclanthology.org/N19-1317)|4|1|4|1|
|henson was born in southern maryland .|[EditNTS](https://aclanthology.org/P19-1331)|4|3|4|3|
|he was born in southern maryland .|[Transformer](http://papers.nips.cc/paper/by-source-2017-3058)|4|2|4|2|
|henson died to eight age , maryland .|[DMASS](https://aclanthology.org/D18-1355)|1|1|1|1|
|he was born in southern maryland .|[BERT](https://aclanthology.org/2020.acl-main.709)|4|2|4|2|


## 文献情報

- 廣中勇希, 井川朋樹, 梶原智之, 二宮崇. **QENTS：テキスト平易化の品質推定のためのデータセット.** 言語処理学会第28回年次大会, 2022.
