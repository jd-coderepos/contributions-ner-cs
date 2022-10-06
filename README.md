# Computer Science Named Entity Recognition in the Open Research Knowledge Graph (CS-NER dataset)


This work proposes a standardized CS-NER task by defining a set of seven _contribution-centric_ scholarly
entities for CS NER viz., _research problem_ , _solution_ , _resource_ , _language_ ,
_tool_ , _method_ , and _dataset_ . 

The main contributions are:

1) Merges annotations for contribution-centric named entities from related work as the following datasets: 
   - The dataset proposed in [Analyzing the Dynamics of Research by Extracting Key Aspects of Scientific Papers](https://aclanthology.org/I11-1001/) (Gupta & Manning, IJCNLP 2011) is the source for [ftd](https://github.com/jd-coderepos/contributions-ner-cs/tree/main/ftd), annotated for both titles and abstracts for the following select entities mapped to our standardized types _focus_ -> _solution_ ; _domain_ -> _research problem_ ; and _technique_ -> _method_ 
   - [scierc](https://github.com/jd-coderepos/contributions-ner-cs/tree/main/scierc),
   - [ncg](https://github.com/jd-coderepos/contributions-ner-cs/tree/main/ncg), and 
   - [pwc](https://github.com/jd-coderepos/contributions-ner-cs/tree/main/pwc).

2) Additionally, supplies a new annotated dataset for the titles and abstracts in the ACL anthology in the [acl repository](https://github.com/jd-coderepos/contributions-ner-cs/tree/main/acl).


### Dataset Statistics



Titles



Abstracts



### Related Work

1) FTD Dataset
[Analyzing the Dynamics of Research by Extracting Key Aspects of Scientific Papers](https://aclanthology.org/I11-1001/) (Gupta & Manning, IJCNLP 2011)

2) SciERC Dataset
[Multi-Task Identification of Entities, Relations, and Coreference for Scientific Knowledge Graph Construction](https://aclanthology.org/D18-1360/) (Luan et al., EMNLP 2018)

3) NCG Dataset
[SemEval-2021 Task 11: NLPContributionGraph - Structuring Scholarly NLP Contributions for a Research Knowledge Graph](https://aclanthology.org/2021.semeval-1.44/) (D’Souza et al., SemEval 2021)


### Citation

```
@article{d2022computer,
  title={Computer Science Named Entity Recognition in the Open Research Knowledge Graph},
  author={D'Souza, Jennifer and Auer, S{\"o}ren},
  journal={arXiv preprint arXiv:2203.14579},
  year={2022}
}
```
