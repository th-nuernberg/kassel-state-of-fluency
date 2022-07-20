---
title: Kassel State of Fluency
site.github.repository_url: https://github.com/th-nuernberg/kassel-state-of-fluency.github.io
---

# KSoF: The Kassel State of Fluency Dataset – A Therapy Centered Dataset of Stuttering
![WordRep](/res/word_rep_spec.jpg)


## Overview

Stuttering is a complex speech disorder that negatively affects an individual’s ability to communicate effectively. 
Persons who stutter (PWS) often suffer considerably under the condition and seek help through therapy.
We created KSoF: The Kassel State of Fluency Dataset, to enable research into the automatic detection of dysfluencies from speech.
It is the biggest available ressource containing German stuttered speech and has fully compatible lables to one of the largest ressources
containing stuttered speech (SEP-28k).
We hope that research into automatic stuttering detection systems will help to enable stutttering self-help applications providing objective feedback. 

The dataset is a unique ressources as, to the best of our knwoledge, it is the only dataset containing speech from PWS that underwent therapy and apply the fluency shaping technique in their speech.
The 5597 clips were labeled with six stuttering-related event types: blocks, prolongations, sound repetitions, word repetitions, interjections, and – specific to therapy – speech modifications.
The audio was recorded during therapy sessions at the [Institut der Kasseler Stottertherapie](https://www.kasseler-stottertherapie.de/). The data will be made available for research purposes upon request.

## Access

The dataset can be requested from [zenodo](https://zenodo.org/record/6801844), after submitting the signed [EULA](KSoF_EULA.pdf).

We also encourage you to explore out our paper on "The Influence of Dataset Partitioning on Dysfluency Detection Systems", improving on the SEP-28k dataset. 
The full extension can be found in the [ml stuttering events dataset extended repository](https://github.com/th-nuernberg/ml-stuttering-events-dataset-extended).

## Literature:
```bibtex
@inproceedings{bayerl_KSoFKasselState_2022,
  title = {{{KSoF}}: {{The Kassel State}} of {{Fluency Dataset}} -- {{A Therapy Centered Dataset}} of {{Stuttering}}},
  booktitle = {Proceedings of the Language Resources and Evaluation Conference},
  author = {Bayerl, Sebastian and {Wolff von Gudenberg}, Alexander and H{\"o}nig, Florian and Noeth, Elmar and Riedhammer, Korbinian},
  year = {2022},
  month = jun,
  pages = {1780--1787},
  publisher = {{European Language Resources Association}},
  address = {{Marseille, France}},
  keywords = {Computer Science - Computation and Language,Electrical Engineering and Systems Science - Audio and Speech Processing},
}

@incollection{bayerl_InfluenceDatasetPartitioning_2022,

  title = {The {{Influence}} of {{Dataset Partitioning}} on {{Dysfluency Detection Systems}}},
  booktitle = {Text, {{Speech}}, and {{Dialogue}}},
  author = {Bayerl, Sebastian P. and Wagner, Dominik and N{\"o}th, Elmar and Bocklet, Tobias and Riedhammer, Korbinian},
  editor = {Sojka, Petr and Kope{\v c}ek, Ivan and Pala, Karel and Hor{\'a}k, Ale{\v s}},
  year = {2022},
  publisher = {{Springer International Publishing}}
}
```
