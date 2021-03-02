Template and example code for paper: [Towards Cross-Lingual Generalization of Translation Gender Bias]() (ACM FaccT 2021)

![figure-3.png](figure-3.png)

## Data files

All files are plain txt, UTF-8 encoding, and each word/sentence was seperated by new line('\n').

**word_list**:<br/>
- occupation word list used in template (187 words): [EN](word_list/occu_en.txt), [KR](word_list/occu_kr.txt), [TL](word_list/occu_tl.txt)
- adjective word list used in template (62 words): [EN](word_list/noun_en.txt)
- noun word list used in template (68 words): [KR](word_list/adj_kr.txt), [TL](word_list/adj_tl.txt)

**template**: sentences given to translators<br/>

- EN
  - [female & noun](template/en-female-noun.txt)
  - [male & noun](template/en-male-noun.txt)
  - [female & occupational](template/en-female-occupation.txt)
  - [male & occupational](template/en-male-occupation.txt)
- KR
  - [female & adjective](template/kr-female-adj.txt)
  - [male & adjective](template/kr-male-adj.txt)
  - [female & occupational](template/kr-female-occupation.txt)
  - [male & occupational](template/kr-male-occupation.txt)
- TL
  - [female & adjective](template/tl-female-adj.txt)
  - [male & adjective](template/tl-male-adj.txt)
  - [female & occupational](template/tl-female-occupation.txt)
  - [male & occupational](template/tl-male-occupation.txt)

**gold_standard**:reference sentences compared with output sentences<br/>



- DE
  - [female & noun](gold_standard/de-female-noun.txt)
  - [male & noun](gold_standard/de-male-noun.txt)
  - [female & occupation](gold_standard/de-female-occupation.txt)
  - [male & occupation](gold_standard/de-male-occupation.txt)
- EN
  - [female & adjective](gold_standard/en-female-adj.txt)
  - [male & adjective](gold_standard/en-male-adj.txt)
  - [female & occupation](gold_standard/en-female-occupation.txt)
  - [male & occupation](gold_standard/en-male-occupation.txt)
- PT
  - [female & noun](gold_standard/pt-female-noun.txt)
  - [male & noun](gold_standard/pt-male-noun.txt)
  - [female & occupation](gold_standard/pt-female-occupation.txt)
  - [male & occupation](gold_standard/pt-male-occupation.txt)


## Evaludation Demo

Both bleu&bertScore were executed on Linux and Python 3.6+.

**bertScore**:<br/>

You can find our example on [Google Colab](https://colab.research.google.com/drive/1wCYv-ViP5vX3InP5NlbXbv6swmOjjjpN#scrollTo=Z3OgidL3RhaF).

Note
- a GPU is usually neccessary.
- the max length is limited to 510(512 after adding cls/sep) as we used bert-base-multilingual-cased as our default model.


**bleu**:<br/>

Our bleu evalation example can be found [here](https://colab.research.google.com/drive/1y0uvMCs_lXqRilE7GI9lRAVbt35BmgBI)

### Authors
\*Won Ik Cho<br/>
\*[Jiwon Kim](https://github.com/SpellOnYou)<br/>
Jaeyeong Yang<br/>
Nam Soo Kim<br/>

\*: equally contributed
