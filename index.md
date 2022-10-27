---
title: "KSoF: The Kassel State of Fluency Dataset – A Therapy Centered Dataset of Stuttering"
link: "dataset_readme"
link_description: "Dataset Readme"
zenodo: "https://zenodo.org/record/6801844"
zenodo_c: "https://zenodo.org/record/6460102"
sep28kE: "https://github.com/th-nuernberg/ml-stuttering-events-dataset-extended"
site.show_links: "true"
---

# KSoF: The Kassel State of Fluency Dataset – A Therapy Centered Dataset of Stuttering
![WordRep](/res/word_rep_spec.jpg)


## Overview

Stuttering is a complex speech disorder that negatively affects an individual’s ability to communicate effectively.
Persons who stutter (PWS) often suffer considerably under the condition and seek help through therapy.
We created the Kassel State of Fluency Dataset (KSoF) to enable research on the automatic detection of dysfluencies from speech.
It is the biggest available labeled resource containing German stuttered speech and has fully compatible labels with one of the largest resources containing stuttered speech (SEP-28k).

We hope that research into automatic stuttering detection systems will help to enable stuttering self-help applications to provide objective feedback.
The dataset is a unique resource as, to the best of our knowledge, it is the only dataset containing speech from PWS that underwent therapy and apply the fluency shaping technique in their speech.
The 5597 clips were labeled with six stuttering-related event types: blocks, prolongations, sound repetitions, word repetitions, interjections, and – specific to therapy – speech modifications. The audio was recorded during therapy sessions at the  [Institut der Kasseler Stottertherapie](https://www.kasseler-stottertherapie.de/) and may be used for research purposes. 

## ACM ComParE Challenge 2022
A subset of the data was featured in the [ACM Multimedia 2022  Computational Paralinguistics Challenge (ComParE) Challenge](http://www.compare.openaudio.eu/2022-2/).
The dataset is based on the full release but only contains a subset with a single label per clip. 
You can find the details in the [challenge paper](https://dl.acm.org/doi/abs/10.1145/3503161.3551591).
## Access

If you are interested in working with the data, please fill out and sign the EULA for the respective release. The [EULA](KSoF_EULA.pdf) full release or the [Challenge Dataset EULA](KSoF_EULA.pdf) (eitherway, must be permanent staff member).
After you submitted the EULA you can proceed to request download access for the full dataset from [zenodo](https://zenodo.org/record/6801844) or the challenge release from [here](https://zenodo.org/record/6460102). 
**Please use the same E-Mail address** or refer to the E-Mail address that was used to submit the EULA.

We also encourage you to explore our paper on **"The Influence of Dataset Partitioning on Dysfluency Detection Systems", improving the SEP-28k dataset.** 
The full extension can be found in the [ml stuttering events dataset extended repository](https://github.com/th-nuernberg/ml-stuttering-events-dataset-extended).

## Literature:
```bibtex
@inproceedings{bayerl_KSoFKasselState_2022,
  title = {KSoF: {The Kassel State of Fluency Dataset -- A Therapy Centered Dataset of Stuttering},
  booktitle = {Proceedings of the Language Resources and Evaluation Conference},
  author = {Bayerl, Sebastian and Wolff von Gudenberg, Alexander and H{\"o}nig, Florian and Noeth, Elmar and Riedhammer, Korbinian},
  year = {2022},
  month = jun,
  pages = {1780--1787},
  publisher = {European Language Resources Association},
  address = {Marseille, France},
  keywords = {Computer Science - Computation and Language,Electrical Engineering and Systems Science - Audio and Speech Processing},
}

@incollection{bayerl_InfluenceDatasetPartitioning_2022,
  title = {The Influence of Dataset Partitioning on Dysfluency Detection Systems},
  booktitle = {Text, Speech, and Dialogue},
  author = {Bayerl, Sebastian P. and Wagner, Dominik and N{\"o}th, Elmar and Bocklet, Tobias and Riedhammer, Korbinian},
  editor = {Sojka, Petr and Kope{\v c}ek, Ivan and Pala, Karel and Hor{\'a}k, Ale{\v s}},
  year = {2022},
  publisher = {Springer International Publishing}
  }

@inproceedings{schuller_ACMMultimedia2022_2022,
  title = {The {{ACM}} Multimedia 2022 Computational Paralinguistics Challenge: {{Vocalisations}}, Stuttering, Activity, \&amp; Mosquitoes},
  booktitle = {Proceedings of the 30th {{ACM}} International Conference on Multimedia},
  author = {Schuller, Björn and Batliner, Anton and Amiriparian, Shahin and Bergler, Christian and Gerczuk, Maurice and Holz, Natalie and Larrouy-Maestri, Pauline and Bayerl, Sebastien and Riedhammer, Korbinian and Mallol-Ragolta, Adria and Pateraki, Maria and Coppock, Harry and Kiskin, Ivan and Sinka, Marianne and Roberts, Stephen},
  date = {2022},
  series = {MM '22},
  publisher ={Association for Computing Machinery},
  doi = {10.1145/3503161.3551591},
}



```
