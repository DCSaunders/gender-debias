# gender-debias
Adaptation datasets and inflected word lists for the paper "Reducing Gender Bias in Neural Machine Translation as a Domain Adaptation Problem" (ACL 2020)

## Walkthrough
We provide a walkthrough for the primary experiments in python notebook format. It is possible to run many experiments such as evaluation and handcrafted dataset adaptation on colab using a CPU. Decoding with SGNMT takes a long time for a single-core machine and so we recommend reproducing those experiments locally and in parallel.

## Models and scripts
The Tensorflow checkpoints for our baseline models can be found here: https://drive.google.com/drive/u/1/folders/1XaWbXQQ8icZZE__fPBOj4dC24oiA3Qtv
Also on the google drive are various utility scripts for lattice rescoring.

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
