---
title: KSoF Dataset Readme
layout: default
link: "index"
link_description: "Home"
---
## Overview
This dataset contains 5597 labeled segments. 
The clips were labeled with six stuttering-related event types and come with additional metadata.
The labels in KSoF are compatible to the lables from the large English dataset SEP-28k, originally created by researches at Apple.
An extended and improved version of the SEP-28k, SEP28k-E can be found on [github](https://github.com/th-nuernberg/ml-stuttering-events-dataset-extended).


## Content
### Files
The release contains this readme file, a copy of the KSoF EULA, a csv file containing the labels, and a foler `segments` which contains an audio file for each clip in the datset.
The filename of the segments matches the column `segment_id` in the `kassel-state-of-fluency-labels.csv` file.
```
KSoF_release
├── Readme.md
├── KSoF_EULA.pdf
├── kassel-state-of-fluency-labels.csv
└── segments
    ├── 0000.wav
    ├── 0001.wav
    ├── 0002.wav
    ├── 0003.wav
    ├── 0004.wav
    ....
```
### Labels

|    |   segment_id |   speaker |   utterance | therapy_status   | gender   | recording_device   | partition   |   Block |   Prolongation |   Sound Repetition |   Word / Phrase Repetition |   No dysfluencies |   Modified/ Speech technique |   Interjection |   Natural pause |   Unintelligible |   Unsure |   No Speech |   Poor Audio Quality |   Music (Background Noise) |
|---:|-------------:|----------:|------------:|:-----------------|:---------|:-------------------|:------------|--------:|---------------:|-------------------:|---------------------------:|------------------:|-----------------------------:|---------------:|----------------:|-----------------:|---------:|------------:|---------------------:|---------------------------:|
|  0 |         0000 |       000 |         000 | nIK              | m        | dg                 | dvel        |       0 |              0 |                  0 |                          0 |                 0 |                            3 |              0 |               0 |                0 |        0 |           0 |                    0 |                          0 |
|  1 |         0001 |       000 |         000 | nIK              | m        | dg                 | dvel        |       1 |              0 |                  0 |                          0 |                 0 |                            1 |              3 |               0 |                0 |        0 |           0 |                    0 |                          0 |
|  ... |         ... |       ... |         ... | ...              | ...        | ...                 | ...        |       ... |              ... |                  ... |                          ... |                 ... |                            ... |              ... |               ... |                ... |        ... |           ... |                    ... |                          ... |

### Columns:
* segment_id:  integer id, denoting a unique segment
* speaker: a numeric speaker label,
* utterance: an id indicationg the original recording the segment was taken from
* therapy_status: indicating the therapy status of a person
  * vIK: recordings from inital interview, before people enter therapy at the Kasseler Stottertherapie
  * nIK: after intensive course, where people learn a speech technique, among other things, in about two weeks time
  * nTh: after therapy is completly done (intensive course, extensive and online supported phase)
* gender
* recording_device:
  * dg: audio from a voice recorder with close talking microphone
  * vat: audio taken from a video camera microphone
  * tm: audio recorded with a table mounted microphone
* partition: data partition in train/dev/test set, for quick evaluation, still we recommend to 5-fold nested cross-validation
* Block, Prolongation, Sound Repetition, Word / Phrase Repetition, No dysfluencies, Modified/ Speech technique, Interjection:
  Label columns, indicating how many (of the 3) labelers, marked the clip as belonging this dysfluency. In the paper we use the majority vote, i.e. a number >= 2 indicates a positivly labeled instance
* Natural pause, Unintelligible, Unsure, No Speech, Poor Audio Quality, Music (Background Noise): Column for meta labels, the approach taken is same as with the dysfluency labels

## Literature
For more details and baseline experiments please see either the [**pre-print on arXiv**](https://arxiv.org/abs/2203.05383) or the link from the [**LREC conference proceedings**](http://www.lrec-conf.org/proceedings/lrec2022/pdf/2022.lrec-1.189.pdf).

### Please cite:

```bibtex
@inproceedings{bayerl_KSoFKasselState_2022,
  title = {KSoF: The Kassel State of Fluency Dataset -- A Therapy Centered Dataset of Stuttering},
  booktitle = {Proceedings of the Language Resources and Evaluation Conference},
  author = {Bayerl, Sebastian Peter and {Wolff von Gudenberg}, Alexander and H{\"o}nig, Florian and Noeth, Elmar and Riedhammer, Korbinian},
  year = {2022},
  month = jun,
  pages = {1780--1787},
  publisher = {European Language Resources Association},
  address = {Marseille, France},
  keywords = {Computer Science - Computation and Language,Electrical Engineering and Systems Science - Audio and Speech Processing},
}
```
### Further reading:
```bibtex
@incollection{bayerl_InfluenceDatasetPartitioning_2022,
  title = {The Influence of Dataset Partitioning on Dysfluency Detection Systems},
  booktitle = {Text, Speech, and Dialogue},
  author = {Bayerl, Sebastian P. and Wagner, Dominik and N{\"o}th, Elmar and Bocklet, Tobias and Riedhammer, Korbinian},
  editor = {Sojka, Petr and Kope{\v c}ek, Ivan and Pala, Karel and Hor{\'a}k, Ale{\v s}},
  year = {2022},
  url = {https://arxiv.org/abs/2206.03400},
  publisher = {Springer International Publishing}
}


@inproceedings{bayerl_DetectingDysfluenciesStuttering_2022,
  title = {Detecting Dysfluencies in Stuttering Therapy Using wav2vec 2.0},
  author = {Bayerl, Sebastian Peter and Wagner, Dominik and N{\"o}th, Elmar and Riedhammer, Korbinian},
  booktitle = {Proc. Interspeech 2022},
  year = {2022},
  url = {https://arxiv.org/abs/2204.03417},
}


@inproceedings{lea_SEP28kDatasetStuttering_2021,
  title = {SEP-28k: A Dataset for Stuttering Event Detection from Podcasts with People Who Stutter},
  shorttitle = {SEP-28k},
  booktitle = {ICASSP 2021 - 2021 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},
  author = {Lea, Colin and Mitra, Vikramjit and Joshi, Aparna and Kajarekar, Sachin and Bigham, Jeffrey P.},
  year = {2021},
  month = jun,
  pages = {6798--6802},
  publisher = {IEEE},
  address = {Toronto, ON, Canada},
  doi = {10.1109/ICASSP39728.2021.9413520},
}


```
