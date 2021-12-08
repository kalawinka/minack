# Mining Acknowledgement Texts in Web of Science
Welcome to the page with the results of the DZHW-funded project **Mining Acknowledgement Texts in Web of Science** (MinAck).

# Please read the following descriptions of the files stored in this repository. 

# accuracy_add_training.csv
Contains the total accuracy of additional training with three algorithms. \
Table with 2 columns: algorithm, value. \
•	algorithm: name of the algorithm used for the training \
•	value: total accuracy of the model 
# comparison_add_training.csv 
Contains performance metrics of additional training with three algorithms. \
Table with 6 columns: algorithm, entity, precision, recall, f1-score, support. \
•	algorithm: name of the algorithm used for the training \
•	entity: entity category \
•	precision: precision value \
•	recall: recall value \
•	f1-score: f1-score value \
•	support: support value 
# accuracy_primary_training.csv
Contains the total accuracy of primary training with three algorithms. \
Table with 3 columns: algorithm, corpus, value \
•	algorithm: name of the algorithm used for the training \
•	corpus: training corpus used for the training \
•	value: total accuracy of the model 
# logs_compare_big.txt
Contains performance metrics of primary training with three algorithms with the corpus no.2 (big). \
Table with 6 columns: algorithm, entity, precision, recall, f1-score, support. \
•	algorithm: name of the algorithm used for the training \
•	entity: entity category \
•	precision: precision value \
•	recall: recall value \
•	f1-score: f1-score value \
•	support: support value 
# logs_compare_small.txt
Contains performance metrics of primary training with three algorithms with the corpus no.1 (small). \
Table with 6 columns: algorithm, entity, precision, recall, f1-score, support. \
•	algorithm: name of the algorithm used for the training \
•	entity: entity category \
•	precision: precision value \
•	recall: recall value \
•	f1-score: f1-score value \
•	support: support value
# 4-class_CoNLL-03_FLAIR_output.csv
Contains the output of a pretrained 4-class NER FLAIR model (CoNLL-03) applied to the training corpus with 1000 acknowledgements texts. \
Table with 4 columns: id, text, label, confidence \
•	id: id of the acknowledgement text \
•	text: extracted entity \
•	label: assigned entity category \
•	confidence: confidence score 
# counts_dataset_small_no1.csv 
Contains number of sentences containing each entity category in the training corpus no.1 (small).\
Table with 4 columns: entity, train, test, dev. \
•	entity: entity category \
•	train: number of sentences containing corresponding entity category in the training set \
•	test: number of sentences containing corresponding entity category in the test set \
•	dev: number of sentences containing corresponding entity category in the validation set 
# counts_dataset_big_no2.csv
Contains number of sentences containing each entity category in the training corpus no.2 (big). \
Table with 4 columns: entity, train, test, dev. \
•	entity: entity category \
•	train: number of sentences containing corresponding entity category in the training set \
•	test: number of sentences containing corresponding entity category in the test set \
•	dev: number of sentences containing corresponding entity category in the validation set 
# train_small_no1.csv, test_small_no1.csv, dev_small_no1.csv 
Contain annotated training, test and validation sets of the corpus no.1 (small) in the csv format. \
Tables with 8 columns: id, txt, GRNB, FUND, IND, UNI, COR, MISC \
•	id: id of the acknowledgement text \
•	txt: sentence of the acknowledgement text \
•	GRNB: acknowledged entity which falls into grant number category \
•	FUND: acknowledged entity which falls into funding agency category \
•	IND: acknowledged entity which falls into person category \
•	UNI: acknowledged entity which falls into university category \
•	COR: acknowledged entity which falls into corporation category \
•	MISC acknowledged entity which falls into miscellaneous category 
# train_big_no2.csv, test_ big_no2.csv, dev_ big_no2.csv 
Contain annotated training, test and validation sets of the corpus no.2 (big) in the csv format. \
Tables with 8 columns: id, txt, GRNB, FUND, IND, UNI, COR, MISC \
•	id: id of the acknowledgement text \
•	txt: sentence of the acknowledgement text \
•	GRNB: acknowledged entity which falls into grant number category \
•	FUND: acknowledged entity which falls into funding agency category \
•	IND: acknowledged entity which falls into person category \
•	UNI: acknowledged entity which falls into university category \
•	COR: acknowledged entity which falls into corporation category \
•	MISC acknowledged entity which falls into miscellaneous category 
# annotated_corpus_1000.csv
Contains annotated corpus with 1000 acknowledgements texts. \
Table with 9 columns: index, id, txt, GRNB, FUND, IND, UNI, COR, MISC \
•	Index: row index \
•	id: id of the acknowledgement text \
•	txt: sentence of the acknowledgement text \
•	GRNB: acknowledged entity which falls into grant number category \
•	FUND: acknowledged entity which falls into funding agency category \
•	IND: acknowledged entity which falls into person category \
•	UNI: acknowledged entity which falls into university category \
•	COR: acknowledged entity which falls into corporation category \
•	MISC acknowledged entity which falls into miscellaneous category 
# wos_disciplines_full.csv
Contains list with full WoS classification of disciplines and scientific domains. \
Table with 2 columns: PK_CLASSIFICATIONS, CLASSIFICATION \
•	PK_CLASSIFICATIONS: id of the discipline \
•	CLASSIFICATION: name of the discipline 
# wos_selected_disciplines.csv
Contains list of disciplines chosen for the acknowledgements corpus. \
Table with 3 columns: PK_CLASSIFICATIONS, CLASSIFICATION, SCI_FIELD \
•	PK_CLASSIFICATIONS: id of the discipline \
•	CLASSIFICATION: name of the discipline \
•	SCI_FIELD: name of the scientific domain 
# counts_disciplines_total.csv
Contains different counts of records in the chosen scientific domains.\
Table with 6 columns: scientific domain, total scientific domain, # disciplines, # records to choose from each discipline (planned), # records in corpus(planned), # records in corpus(real unique values) \
•	scientific domain: name of the scientific domain \
•	total scientific domain: total number of records in WoS in corresponding scientific domain \
•	# disciplines: number of disciplines per scientific domain \
•	# records to choose from each discipline (planned): approximate number of articles, which should have been picked up from each discipline, in order to create a well-balanced corpus \
•	# records in corpus(planned): planned number of records in the acknowledgements corpus from each scientific domain \
•	# records in corpus(real unique values): real number of records (unique for each discipline) in the acknowledgements corpus from each scientific domain
# counts_disciplines_single_discipline.csv
Contains different counts of records for each discipline in each scientific domain. \
Table with 9 columns: PK_CLASSIFICATIONS, CLASSIFICATION,SCI_FIELD, # records 2014-2019 Eng, # records 2014-2019 Eng with fund info, # records 2014-2019 Eng with Ackn, # records 2014-2019 Eng filtered by pub/doctype, # records 2014-2019 Eng with Ackn filtered by pub/doctype, #records in acknowledgemnts corpus (real unique values) \
•	PK_CLASSIFICATIONS: id of the discipline \
•	CLASSIFICATION: name of the discipline \
•	SCI_FIELD: name of the scientific domain \
•	# records 2014-2019 Eng: number of records published between 2014 and 2019 in English \
•	# records 2014-2019 Eng with fund info: number of records published between 2014 and 2019 in English, which contain indexed funding information \
•	# records 2014-2019 Eng with Ackn: Eng with fund info: number of records published between 2014 and 2019 in English, which contain acknowledgement \
•	# records 2014-2019 Eng filtered by pub/doctype: number of records published between 2014 and 2019 in English, of type article or review, published in a journal \
•	# records 2014-2019 Eng with Ackn filtered by pub/doctype: number of records published between 2014 and 2019 in English, of type article or review, published in a journal, which contain acknowledgement \
•	#records in acknowledgemnts corpus (real unique values): number of unique records chosen for the acknowledgements corpus
# analysis_raw_entity_comp.csv, analysis_raw_entity_soc.csv, analysis_raw_entity_eco.csv, analysis_raw_entity_ocean.csv, analysis_raw_entity_total.csv
Contain analysis of the raw NER tagger output (without disambiguation): frequencies of entities per discipline. Comp stands for computer science, eco stands for economics, soc stands for sociology, ocean stands for oceanography, total is all disciplines together. \
Tables with 10 columns: FUND, freq, MISC, freq.1, UNI, freq.2, COR, freq.3, IND, freq.4 \
•	freq-frq.4: frequencies of occurrence of acknowledged entity \
•	FUND: acknowledged entity which falls into funding agency category \
•	IND: acknowledged entity which falls into person category \
•	UNI: acknowledged entity which falls into university category \
•	COR: acknowledged entity which falls into corporation category \
•	MISC acknowledged entity which falls into miscellaneous category 
# analysis_raw_labels_frequency.csv 
Contains frequencies of occurrences of different categories of entities in different scientific domains. \
Table with 6 columns: entity, all disciplines, oceanography, economics, sociology, computer science. \
•	entity: entity category \
•	all disciplines: number of occurrences for all disciplines \
•	oceanography: number of occurrences for oceanography \
•	economics: number of occurrences for economics \
•	sociology: number of occurrences for sociology \
•	computer science: number of occurrences for computer science 
# diasmbiguation_patterns_fund.csv
Contains different writing variants and abbreviations for funding organizations. Used for disambiguation of acknowledged entities. \
Table with 3 columns: text, abbreviation, full \
•	text: one of the writing variants of the acknowledged entity \
•	abbreviation: corresponding abbreviation \
•	full: correct writing variant of the acknowledged entity
# diasmbiguation_patterns_uni.csv
Contains different writing variants and abbreviations for universities. Used for disambiguation of acknowledged entities. \
Table with 3 columns: text, abbreviation, full \
•	text: one of the writing variants of the acknowledged entity \
•	abbreviation: corresponding abbreviation \
•	full: correct writing variant of the acknowledged entity
# analysis_ disambiguated_entity_comp.csv, analysis_ disambiguated_entity_soc.csv, analysis_ disambiguated_entity_eco.csv, analysis_ disambiguated_entity_ocean.csv, analysis_ disambiguated_entity_total.csv
Contain analysis of the disambiguated NER tagger output: frequencies of entities per discipline. Comp stands for computer science, eco stands for economics, soc stands for sociology, ocean stands for oceanography, total is all disciplines together. \
Tables with 10 columns: FUND, freq, MISC, freq.1, UNI, freq.2, COR, freq.3, IND, freq.4 \
•	freq-frq.4: frequencies of occurrence of acknowledged entity \
•	FUND: acknowledged entity which falls into funding agency category \
•	IND: acknowledged entity which falls into person category \
•	UNI: acknowledged entity which falls into university category \
•	COR: acknowledged entity which falls into corporation category \
•	MISC acknowledged entity which falls into miscellaneous category 
# [corpus_1000_without_duplicates.csv.gz](https://gesisbox.gesis.org/index.php/s/7AgzPcF2X3CgSYA)
Contains corpus with 1000 acknowledgements texts, which were used to create the training corpora. \
Table with 4 columns: fk_items, fundingorganization, grantnumber, granttext \
•	fk_items: id of the acknowledgement text \
•	fundingorganization: indexed funding agency \
•	grantnumber: indexed grant number \
•	granttext: acknowledgement text
# train_big.txt, test_big.txt, dev_big.txt
Contain annotated training, test and validation sets of the corpus no.2 (big) in the IOB2-format. Words marked B- indicate the beginning of the annotated chunk, words marked I- are inside the annotated chunk and words marked O are outside the annotated chunk. 
# train_small.txt, test_ small.txt, dev_ small.txt 
Contain annotated training, test and validation sets of the corpus no.1 (small) in the IOB2-format. Words marked B- indicate the beginning of the annotated chunk, words marked I- are inside the annotated chunk and words marked O are outside the annotated chunk.
# [cor_disamb2.csv.gz](https://gesisbox.gesis.org/index.php/s/GMMwNFSc9BXsT7Y), [fund_disamb2.csv.gz](https://gesisbox.gesis.org/index.php/s/XZNYJSWJbSP8JkG), [ind_disamb2.csv.gz](https://gesisbox.gesis.org/index.php/s/FXMdfFJE7D7iWDd), [misc_disamb2.csv.gz](https://gesisbox.gesis.org/index.php/s/3wdG58ScQMCgbYz), [uni_disamb2.csv.gz](https://gesisbox.gesis.org/index.php/s/9WMQz6DBaKHjott)
Contain disambiguated NER model output. File with the core_ prefix in the file name contains entities of the COR (corporation) category, fund_ contains entities of the FUND (funding organization) category, ind_ contains entities of the IND (person) category, misc_ contains entities of the MISC (miscellaneous) category, uni_ contains entities of the UNI (university) category. \
Table with 9 columns: index, pk_items, entity, label, confidence, doi, fk_classifications, id, disamb \
•	index: row index \
•	pk_items: id of the acknowledgement text \
•	entity: extracted acknowledged entity \
•	label: label: assigned entity category \
•	confidence: confidence score \
•	doi: doi of the article to which the acknowledgment text belongs \
•	fk_classifications: id of the discipline \
•	id: id of the extracted entity, assigned during disambiguation. Consists of index + pk_items \
•	disamb: disambiguated acknowledged entity
# [acknowledgments_ner_imp.csv.gz](https://gesisbox.gesis.org/index.php/s/e8fTos84Wf2fmje ) 
Contains NER model output. \
Table with 6 columns: pk_items, entity, label, confidence, doi, fk_classifications \
•	pk_items: id of the acknowledgement text \
•	entity: extracted acknowledged entity \
•	label: label: assigned entity category \
•	confidence: confidence score \
•	doi: doi of the article to which the acknowledgment text belongs \
•	fk_classifications: id of the discipline 
# [final-model.pt](https://gesisbox.gesis.org/index.php/s/w96ptRqsoXEpjQk ) 
Contains FLAIR NER model with the best accuracy (FLAIR Embeddings) trained on the big corpus.
# [corpus2.csv.gz](https://gesisbox.gesis.org/index.php/s/qXCZkNYzfW3kGkz )
Contains acknowledgments corpus, which was analyzed with the NER model. \
Table with columns: pk_items, doi, TO_CHAR(GRT.GRANTTEXT), article_title, doctype, pubtype, pubyear, fk_classifications \
•	pk_items: id of the acknowledgement text \
•	doi: doi of the article to which the acknowledgment text belongs \
•	TO_CHAR(GRT.GRANTTEXT): acknowledgment text \
•	article_title: name of the article to which the acknowledgment text belongs \
•	doctype: article document type \
•	pubtype: article publishing type \
•	pubyear: article publishing year \
•	fk_classifications: id of the discipline







