<p align="center"><img src="https://github.com/kalawinka/minack/blob/main/logo_round3.png" width="200" height="130"></p>

# Mining Acknowledgement Texts in Web of Science

Welcome to the homepage of the DZHW-funded project **Mining Acknowledgement Texts in Web of Science** (MinAck).

## Introduction
The aim of the project is to conduct an analysis of acknowledgment texts from the [Web of Science (WoS)](https://clarivate.com/webofsciencegroup/solutions/web-of-science/) using the [FLAIR NLP Framework](https://github.com/flairNLP/flair). Acknowledgments contain information about technical, instrumental, and financial support together with mentions of intellectual and conceptual support (Diaz-Faes & Bordons, 2017; Giles & Councill, 2004). The focus of the project is the detection and quantitative analysis of acknowledged entities, i.e., named entity recognition (NER) task in a larger corpus of WoS articles which include acknowledgements.

An acknowledged entity is an object of acknowledgment which could be names and surnames of individuals (also abbreviations), names of institutions and organizations, numbers, and ids of grants.

The analysis of acknowledgments is particularly interesting as acknowledgments may give an insight on such aspects of scientific society as reward systems, collaboration structures, and hidden research trends (Giles & Councill, 2004).

In our project, the FLAIR NLP Framework will be used to perform the acknowledged entity recognition task. FLAIR is “*an NLP framework designed to facilitate training and distribution of state-of-the-art sequence labeling, text classification and language models*” (Akbik et al.). FLAIR is open-sourced and built on [PyTorch](https://pytorch.org/), which is an open source machine learning library.

## Project outline
As WoS contains millions of metadata records, the data chosen for the present study will be restricted by year and discipline. We plan to analyze articles from four different scientific disciplines published from 2014 to 2019: articles from the social sciences (sociology and economics) and oceanography and computer science to compare. The entire dataset will contain approx. 200,000 entries, i.e., 50,000 from each scientific domain.

Two of the aims of the present project are to extract acknowledged entities from the samples set and ascribe them to different categories (described below). FLAIR provides the possibility to create a custom NER tagger (GitHub, 2021). Creating a custom NER tagger will allow us to accomplish these two aims (acknowledged entity recognition and acknowledged entities classification) in one step. As a result, the model should be able to recognize five entity types: **funding agencies** (FUND), **corporations** (COR), **universities** (UNI), **individuals** (IND) and **grant numbers** (GRNB).

## Contact
* Nina Smirnova, nina.smirnova@gesis.org
* Philipp Mayr, philipp.mayr@gesis.org

## Funding
German Centre for Higher Education Research and Science Studies (DZHW); Start: August 2021; Duration: 4 Months

## References
1) Akbik, A. (n.d.). The Flair NLP Framework. Retrieved from: https://alanakbik.github.io/flair.html.

2) Diaz-Faes, A. A. & Bordons, M. (2017). Making visible the invisible through the analysis of acknowledgements
in the humanities. Aslib Journal of Information Management, 69(5), 576–590. Retrieved from:
https://arxiv.org/pdf/1706.06334.

3) Giles, C. L. & Councill, I. G. (2004). Who gets acknowledged: measuring scientific contributions through
automatic acknowledgment indexing. Proceedings of the National Academy of Sciences of the United States
of America, 101(51), 17599–17604.

4) GitHub (2021). Importing custom NER tagger into flair and using.predict. Using BIOUL tagging scheme. ·
Issue #787 · flairNLP/flair. Retrieved from: https://github.com/flairNLP/flair/issues/787 (16 January, 2021).
