# QENTS: Corpus for Quality Estimation of Neural Text Simplification

We released a dataset to build quality estimation models for English text simplification.

- Our dataset consists of 10,770 sentences from the Newsela corpus, including output sentences from 10 typical text simplification models.
- We manually evaluated these sentences from four perspectives: Grammaticality,
Meaning preservation, Simplicity, and Overall quality on a four-point scale (1: worst, 4: best). 


## Examples

Source：Henson , who lived to age 93 , was born in southern Maryland .

||Model|Grammaticality|Meaning Preservation|Simplicity|Overall Quality|
| :--- | :---: | :---: | :---: | :---: | :---: |
|henson was born in maryland and lived to be 93 years old .|Reference|4|3|3|4|
|henson , who lived to age , for instance , was born in maryland .|[PBMT-R](https://aclanthology.org/P12-1107)|1|1|1|1|
|henson lived was born .|[Hybrid](https://aclanthology.org/P14-1041)|1|1|1|1|
|henson was born in southern maryland .|[EncDecA](https://aclanthology.org/D15-1166)|4|3|4|3|
|henson lived to age 93 .|[DRESS](https://aclanthology.org/D17-1062)|4|3|4|3|
|henson lived in maryland .|[S2S-All-FA](https://aclanthology.org/N19-1317)|4|1|4|1|
|henson was born in southern maryland .|[EditNTS](https://aclanthology.org/P19-1331)|4|3|4|3|
|he was born in southern maryland .|[Transformer](http://papers.nips.cc/paper/by-source-2017-3058)|4|2|4|2|
|henson died to eight age , maryland .|[DMASS](https://aclanthology.org/D18-1355)|1|1|1|1|
|he was born in southern maryland .|[BERT](https://aclanthology.org/2020.acl-main.709)|4|2|4|2|


## References

- 廣中勇希, 井川朋樹, 梶原智之, 二宮崇. **QENTS：テキスト平易化の品質推定のためのデータセット.** 言語処理学会第28回年次大会, 2022.
