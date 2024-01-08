# Computer Science Named Entity Recognition in the Open Research Knowledge Graph (CS-NER dataset)

### 1) About

This work proposes a standardized CS-NER task by defining a set of seven _contribution-centric_ scholarly
entities for CS NER viz., _research problem_ , _solution_ , _resource_ , _language_ ,
_tool_ , _method_ , and _dataset_ . 

The main contributions are:

1) Merges annotations for contribution-centric named entities from related work as the following datasets: 
   - The dataset proposed in [Analyzing the Dynamics of Research by Extracting Key Aspects of Scientific Papers](https://aclanthology.org/I11-1001/) (Gupta & Manning, IJCNLP 2011) is the source for [ftd](https://github.com/jd-coderepos/contributions-ner-cs/tree/main/ftd), annotated for both titles and abstracts for the following select entities mapped to our standardized types _focus_ -> _solution_ ; _domain_ -> _research problem_ ; and _technique_ -> _method_ 
   - The dataset proposed in [Multi-Task Identification of Entities, Relations, and Coreference for Scientific Knowledge Graph Construction](https://aclanthology.org/D18-1360/) (Luan et al., EMNLP 2018) is the source for [scierc](https://github.com/jd-coderepos/contributions-ner-cs/tree/main/scierc), annotated for abstracts for the following select entities with mappings _task_ -> _research problem_
   - The dataset proposed in [SemEval-2021 Task 11: NLPContributionGraph - Structuring Scholarly NLP Contributions for a Research Knowledge Graph](https://aclanthology.org/2021.semeval-1.44/) (D’Souza et al., SemEval 2021) is the source for [ncg](https://github.com/jd-coderepos/contributions-ner-cs/tree/main/ncg), annotated for both titles and abstracts for _research problem_
   - https://paperswithcode.com/ as the [pwc](https://github.com/jd-coderepos/contributions-ner-cs/tree/main/pwc) annotated for both titles and abstracts for _task_ -> _research problem_ and _method_ entities.

2) Additionally, supplies a new annotated dataset for the titles in the ACL anthology in the [acl repository](https://github.com/jd-coderepos/contributions-ner-cs/tree/main/acl) 
where titles are annotated with all seven entities.


### 2) Dataset Statistics for [full dataset](https://github.com/jd-coderepos/contributions-ner-cs/tree/main/full%20dataset)

Please note the numbers below reflect the total annotated entities. They do not reflect the unique set of annotated entities.

#### Titles

`train.data`

| NER | Count |
| --- | --- |
| solution | 18,924 |
| research problem | 15,646 |
| method | 8,854 |
| resource | 7,346 |
| tool | 1,718 |
| language | 1,141 |
| dataset | 882 |

`dev.data`

| NER | Count |
| --- | --- |
| solution | 1,072 |
| research problem | 989 |
| method | 574 |
| resource | 439 |
| tool | 93 |
| language | 50 |
| dataset | 39 |

`test.data`

| NER | Count |
| --- | --- |
| solution | 8,316 |
| research problem | 4,070 |
| resource | 3,226 |
| method | 2,768 |
| tool | 743 |
| language | 499 |
| dataset | 228 |

#### Abstracts

`train-abs.data`

| NER | Count |
| --- | --- |
| method | 10,992 |
| research problem | 7,485 |

`dev-abs.data`

| NER | Count |
| --- | --- |
| method | 719 |
| research problem | 603 |

`test-abs.data`

| NER | Count |
| --- | --- |
| method | 2,723 |
| research problem | 2,100 |

The remaining repositories have specialized README files with the respective dataset statistics.

### 3) Citation

If this work inspires your further research, please consider citing our [ICADL 2022](https://icadl.net/icadl2022/) proceedings paper.

```
@InProceedings{10.1007/978-3-031-21756-2_3,
author="D'Souza, Jennifer
and Auer, S{\"o}ren",
editor="Tseng, Yuen-Hsien
and Katsurai, Marie
and Nguyen, Hoa N.",
title="Computer Science Named Entity Recognition in the Open Research Knowledge Graph",
booktitle="From Born-Physical to Born-Virtual: Augmenting Intelligence in Digital Libraries",
year="2022",
publisher="Springer International Publishing",
address="Cham",
pages="35--45",
abstract="Domain-specific named entity recognition (NER) on Computer Science (CS) scholarly articles is an information extraction task that is arguably more challenging for the various annotation aims that can hamper the task and has been less studied than NER in the general domain.  Given that significant progress has been made on NER, we anticipate that scholarly domain-specific NER will receive increasing attention in the years to come. Currently, progress on CS NER -- the focus of this work -- is hampered in part by its recency and the lack of a standardized annotation aims for scientific entities/terms. Directly addressing these issues, this work proposes a standardized task by defining a set of seven contribution-centric scholarly entities for CS NER viz., research problem, solution, resource, language, tool, method, and dataset.",
isbn="978-3-031-21756-2"
}
```



Preprint

```
@article{d2022computer,
  title={Computer Science Named Entity Recognition in the Open Research Knowledge Graph},
  author={D'Souza, Jennifer and Auer, S{\"o}ren},
  journal={arXiv preprint arXiv:2203.14579},
  year={2022}
}
```

### 4) Additional resources

#### CS NER Software trained on the dataset in this repository

Codebase: https://gitlab.com/TIBHannover/orkg/nlp/orkg-nlp-experiments/-/tree/master/orkg_cs_ner

Service URL - REST API: https://orkg.org/nlp/api/docs#/annotation/annotates_paper_annotation_csner_post

Service URL - PyPi: https://orkg-nlp-pypi.readthedocs.io/en/latest/services/services.html#cs-ner-computer-science-named-entity-recognition 

