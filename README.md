# gender-debias
Adaptation datasets and inflected word lists for the paper "Reducing Gender Bias in Neural Machine Translation as a Domain Adaptation Problem" (ACL 2020)


## Adaptation data
We provide the handcrafted and handcrafted-nooverlap sets adaptation sets described in section 2.2.1 of the paper, in English-German, English-Spanish and English-Hebrew. These are small (388 parallel sentence pairs) gender-balanced datasets. 

All target language sentences were constructed by an MT first-pass translation from English followed by manual checking by a non-native speaker: we apologize and welcome corrections for any mistranslations!

## Inflection lists
In section 2.3.2 of the paper, we describe a lattice rescoring scheme for biased translations. This involves building a gender-inflected search space for every hypothesis, which itself requires a mapping of target language words to their inflected forms. 

We provide our gender-inflected lists with the caution that they were constructed on large vocabulary lists using simple heuristics with an eye towards over-generation, and should not be considered grammatically reliable.

## Citing

```
@InProceedings{saunders2020genderbias,
  author    = {Danielle Saunders and Bill Byrne},
  title     = {Reducing Gender Bias in Neural Machine Translation as a Domain Adaptation Problem},
  booktitle = {ACL},
  month     = {July},
  year      = {2020},
  publisher = {Association for Computational Linguistics}
}
```
