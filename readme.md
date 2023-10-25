# SpeechRealization

Goals:
1) Understand empirical markers of gender & accent in speech
2) Use literature to dissect their interaction in terms of articulation and perception

## Conversational Datasets (Multilingual):
I already resampled these to 16kHz, mono-channel. You can interact with them with the huggingface datasets API.

### Install Datasets
```
pip install datasets
```

### Save data to a dictionary:
```
import datasets
from datasets import load_dataset

dsets = ['NathanRoll/TalkBank_CA_wM_GCSAusE','NathanRoll/TalkBank_CA_wM_CORAAL','NathanRoll/TalkBank_CA_wM_CLAPI','NathanRoll/TalkBank_CA_wM_Croatian',
            'NathanRoll/TalkBank_CA_wM_Bergmann','NathanRoll/TalkBank_CA_wM_TaiwanHakka','NathanRoll/TalkBank_CA_wM_SBCSAE']

for j in dsets:
  d[j] = load_dataset(j)
```

Datasets:

```
@inproceedings{commonvoice2020,
  author = {Ardila, R. and Branson, M. and Davis, K. and Henretty, M. and Kohler, M. and Meyer, J. and Morais, R. and Saunders, L. and Tyers, F. M. and Weber, G.},
  title = {Common Voice: A Massively-Multilingual Speech Corpus},
  booktitle = {Proceedings of the 12th Conference on Language Resources and Evaluation (LREC 2020)},
  pages = {4211--4215},
  year = 2020
}

@incollection{Bergmann1993,
  author    = {Bergmann, J.},
  title     = {Alarmiertes verstehen: Kommunikation in Feuerwehrnotrufen. Wirklichkeit im Deutungsprozeß},
  booktitle = {Verstehen und Methoden in den Kultur-und Sozialwissenschaften},
  editor    = {Jung, T. and Müller-Doohm, S.},
  pages     = {283-328},
  year      = {1993},
  publisher = {Suhrkamp},
  address   = {Frankfurt aM}
}

@online{CABNC2015,
  author  = {Saul Albert and Laura E. de Ruiter and J.P. de Ruiter},
  title   = {CABNC: the Jeffersonian transcription of the Spoken British National Corpus},
  year    = {2015},
  url     = {https://saulalbert.github.io/CABNC/}
}

@inbook{CLAPI2016,
  author    = {Baldauf-Quilliatre, H. and Colon de Carvajal, I. and Etienne, C. Jouin-Chardon and Teston-Bonnard, S. Traverso and V.},
  title     = {CLAPI, une base de données multimodale pour la parole en interaction: apports et dilemmes},
  booktitle = {Corpus de français parlés et français parlés des corpus},
  editor    = {Avanzi, M. and Béguelin, M.-J. and Diémoz, F.},
  series    = {Cahiers Corpus},
  year      = {2016}
}

@inbook{CORAAL2022,
  author    = {Kendall, T. and Farrington, C.},
  title     = {Managing Sociolinguistic Data with the Corpus of Regional African American Language (CORAAL)},
  booktitle = {The Open Handbook of Linguistic Data Management},
  pages     = {185},
  year      = {2022}
}

@article{Croatian2016,
  author    = {Kuvač Kraljević, Jelena and Hržica, Gordana},
  title     = {Croatian Adult Spoken Language Corpus (HrAL)},
  journal   = {Fluminensia: Journal for philological research},
  volume    = {28},
  number    = {2},
  year      = {2016},
  url       = {http://fluminensia.ffri.hr/en/clanak?id=1466.html}
}

@inbook{GCSAusE2013,
  author    = {Haugh, Michael and Chang, Wei-Lin Melody},
  title     = {Collaborative creation of spoken language corpora},
  booktitle = {Pragmatics and Language Learning. Volume 13},
  editor    = {Greer, Tim and Kite, Yuriko and Tatsuki, Donna},
  pages     = {133-159},
  year      = {2013},
  publisher = {National Foreign Language Resource Center, University of Hawai’i, Honolulu}
}

@misc{SBCSAE2000,
  author    = {Du Bois, John W. and Chafe, Wallace L. and Meyer, Charles and Thompson, Sandra A. and Englebretson, Robert and Martey, Nii},
  title     = {Santa Barbara corpus of spoken American English, Parts 1-4},
  year      = {2000-2005},
  publisher = {Linguistic Data Consortium},
  address   = {Philadelphia}
}

@inbook{TaiwanHakka2017,
  author    = {Chui, Kawai and Lai, Huei-ling and Chan, Hui-Chen},
  title     = {The Taiwan Spoken Chinese Corpus},
  booktitle = {Encyclopedia of Chinese Language and Linguistic},
  editor    = {Sybesma, Rint},
  pages     = {257-259},
  year      = {2017},
  publisher = {Brill},
  address   = {Boston, USA}
}

```
