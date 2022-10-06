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

2) Additionally, supplies a new annotated dataset for the titles and abstracts in the ACL anthology in the [acl repository](https://github.com/jd-coderepos/contributions-ner-cs/tree/main/acl) 
where titles are annotated with all seven entities, while abstracts are annotated with _research problem_ and _method_ entities.


### 2) Dataset Statistics for [full dataset](https://github.com/jd-coderepos/contributions-ner-cs/tree/main/full%20dataset)

Titles

`train.data`

| NER | Count |
| --- | --- |
| solution | 65,213 |
| research problem | 43,033 |
| resource | 19,759 |
| method | 19,645 |
| tool | 4,856 |
| dataset | 4,062 |
| language | 1,704 |

`dev.data`

| NER | Count |
| --- | --- |
| solution | 3,685 |
| research problem | 2,717 |
| resource | 1,224 |
| method | 1,172 |
| tool | 264 |
| dataset | 191 |
| language | 79 |

`test.data`

| NER | Count |
| --- | --- |
| solution | 29,287 |
| research problem | 11,093 |
| resource | 8,511 |
| method | 7,009 |
| tool | 2,272 |
| dataset | 947 |
| language | 690 |

Abstracts

`train-abs.data`

| NER | Count |
| --- | --- |
| research problem | 15,498 |
| method | 12,932 |

`dev-abs.data`

| NER | Count |
| --- | --- |
| research problem | 1,450 |
| method | 839 |

`test-abs.data`

| NER | Count |
| --- | --- |
| research problem | 4,123 |
| method | 3,170 |


### 3) Citation

```
@article{d2022computer,
  title={Computer Science Named Entity Recognition in the Open Research Knowledge Graph},
  author={D'Souza, Jennifer and Auer, S{\"o}ren},
  journal={arXiv preprint arXiv:2203.14579},
  year={2022}
}
```
