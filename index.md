<p align="center"><img src="https://github.com/kalawinka/minack/blob/media/logo_round3.png?raw=true" width="250" height="130"></p>

# Mining Acknowledgement Texts in Web of Science

Welcome to the homepage of the DZHW-funded project **Mining Acknowledgement Texts in Web of Science** (MinAck).

## Introduction
The aim of the project is to conduct an analysis of acknowledgment texts from the [Web of Science (WoS)](https://clarivate.com/webofsciencegroup/solutions/web-of-science/) using the [FLAIR NLP Framework](https://github.com/flairNLP/flair). Acknowledgments contain information about technical, instrumental, and financial support together with mentions of intellectual and conceptual support (Diaz-Faes & Bordons, 2017; Giles & Councill, 2004). The focus of the project is the detection and quantitative analysis of acknowledged entities, i.e., named entity recognition (NER) task in a larger corpus of WoS articles which include acknowledgements.

An acknowledged entity is an object of acknowledgment which could be names and surnames of individuals (also abbreviations), names of institutions and organizations, numbers, and ids of grants.

The analysis of acknowledgments is particularly interesting as acknowledgments may give an insight on such aspects of scientific society as reward systems, collaboration structures, and hidden research trends (Giles & Councill, 2004).

In our project, the FLAIR NLP Framework is used to perform the acknowledged entity recognition task. FLAIR is “*an NLP framework designed to facilitate training and distribution of state-of-the-art sequence labeling, text classification and language models*” (Akbik et al., 2019). FLAIR is open-sourced and built on [PyTorch](https://pytorch.org/), which is an open source machine learning library.

## Project outline
As WoS contains millions of metadata records, the data chosen for the present study will be restricted by year and discipline. We plan to analyze articles from four different scientific disciplines published from 2014 to 2019: articles from the social sciences (sociology and economics) and oceanography and computer science to compare. The entire dataset will contain approx. 200,000 entries, i.e., 50,000 from each scientific domain.

Two of the aims of the present project are to extract acknowledged entities from the samples set and ascribe them to different categories (described below). FLAIR provides the possibility to create a custom NER tagger (GitHub, 2021). Creating a custom NER tagger will allow us to accomplish these two aims (acknowledged entity recognition and acknowledged entities classification) in one step. As a result, the model should be able to recognize sic entity types: **funding agencies** (FUND), **corporations** (COR), **universities** (UNI), **individuals** (IND), **grant numbers** (GRNB) and **miscellaneous** (MISC).

## Publications and Talks
* Mining Acknowledgement Texts in Web of Science. Poster presented at [SciNLP 2021](https://scinlp.org/): 2nd Workshop on Natural Language Processing for Scientific Text. [PDF](https://github.com/kalawinka/minack/blob/conference/abstract_MinAck_SCINLP21_final.pdf), [Poster](https://github.com/kalawinka/minack/blob/conference/poster_sci_nlp.pdf), [Talk](https://youtu.be/1b0Dso-YOAI)
* Smirnova, N. and P. Mayr 2022. Evaluation of embedding models for automatic extraction and classification of acknowledged entities in scientific documents. In C. Zhang, P. Mayr, W. Lu, and Y. Zhang (Eds.), Proceedings of the 3rd Workshop on Extraction and Evaluation of Knowledge Entities from Scientific Documents (EEKE 2022), pp. 48–55. CEUR, Aachen. http://ceur-ws.org/Vol-3210/paper5.pdf

## Demo
You can try our NER tagger in [huggingface](https://huggingface.co/kalawinka/flair-ner-acknowledgments) or in this [demo](https://colab.research.google.com/drive/1Wz4ae5c65VDWanY3Vo-fj__bFjn-loL4?usp=sharing).

This demo is an interactive notebook built with the [Google Colab](https://colab.research.google.com/). Two options are available, you can try the model with our example of acknowledgement or you can type in your own acknowledgement text. To use the demo just launch one cell after another and follow the instructions, written in the notebook.

Example of the FLAIR NER tagger trained with the Flair Embeddings model:
![Demo image](https://github.com/kalawinka/minack/blob/media/Screenshot%20(62).png?raw=true)
In the first line we created a Sentence object from the sentence: *“This work was supported by State Key Lab of Ocean Engineering Shanghai Jiao Tong University and financially supported by China National Scientific and Technology Major Project (Grant No. 2016ZX05028-006-009).”* The second line generates spans with labelled acknowledged entities from the Sentence object. The third line demonstrates a gold standard: manually annotated acknowledged entities. 

## Data
The data and the analysis are available [here](https://github.com/kalawinka/minack/tree/results) and [here](https://zenodo.org/record/5776202).

## Contact
* Nina Smirnova, nina.smirnova@gesis.org; ninasmirnova@web.de
* Philipp Mayr, philipp.mayr@gesis.org

## Funding
German Centre for Higher Education Research and Science Studies (DZHW); Start: August 2021; Duration: 4 Months

## References
1) Akbik, A., Bergmann, T., Blythe, D., Rasul, K., Schweter, S. & Vollgraf, R. (2019). FLAIR: An Easy-to-Use Framework for State-of-the-Art NLP (W. Ammar, A. Louis, & N. Mostafazadeh, Eds.; pp. 54–59). Association for Computational Linguistics. https://doi.org/10.18653/v1/N19-4010.

2) Diaz-Faes, A. A. & Bordons, M. (2017). Making visible the invisible through the analysis of acknowledgements
in the humanities. Aslib Journal of Information Management, 69(5), 576–590. Retrieved from:
https://arxiv.org/pdf/1706.06334.

3) Giles, C. L. & Councill, I. G. (2004). Who gets acknowledged: measuring scientific contributions through
automatic acknowledgment indexing. Proceedings of the National Academy of Sciences of the United States
of America, 101(51), 17599–17604.

4) GitHub (2021). Importing custom NER tagger into flair and using.predict. Using BIOUL tagging scheme. ·
Issue #787 · flairNLP/flair. Retrieved from: https://github.com/flairNLP/flair/issues/787 (16 January, 2021).
