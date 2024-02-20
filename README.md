# hhuEDOS2023

This repository contains the source code for the models used for hhuEDOS team's submission for <a href="https://codalab.lisn.upsaclay.fr/competitions/7124" target="_blank">SemEval-2023 Shared Task 10, Subtask A “Explainable Detection of Online Sexism (EDOS)"</a>. We ranked 55th out of 84 teams.



## Overview

Listed below are all our methods we experimented with. However, we noticed that our notebook 2 ultimately delivered the best score out of all of our models. Our submitted model uses semi-supervised learning and yieled results with a macro F1 score of 81.85%. 

| Notebook | Description |
| ------------- | ------------- |
| Task_EDOS_Semeval_0_baseline  | Finetuned three pretrained language models, namely BERT, RoBERTa and DistilBERT, with our training data to find a baseline model for further training. |
| Task_EDOS_Semeval_1_imbalanced_data | Augmented our data to balance unequally distributed classes.   |
| Task_EDOS_Semeval_2_semi-supervised | Applied our pretrained language model on additional unlabeled data to augment the dataset and re-train the model. Includes our Error Analysis|
| Task_EDOS_Semeval_3_ML | Applied traditional machine learning methods and test several classifiers with different parameter settings. Features are extracted using TF-IDF.|

## Data

The dataset is provided by the SemEval-2023 Task 10 organizers.

```
@inproceedings{kirkSemEval2023,
title = {{SemEval}-2023 {Task} 10: {Explainable} {Detection} of {Online} {Sexism}},
url = {http://arxiv.org/abs/2303.04222},
doi = {10.48550/arXiv.2303.04222},
author = {Kirk, Hannah Rose and Yin, Wenjie and Vidgen, Bertie and Röttger, Paul},
booktitle = {Proceedings of the 17th {{International Workshop}} on {{Semantic Evaluation}} ({{SemEval-2023}})},
publisher = {{Association for Computational Linguistics}},
year = {2023}
}
```

## How to cite

```
@inproceedings{petersen-etal-2023-hhuedos,
    title = "hhu{EDOS} at {S}em{E}val-2023 Task 10: Explainable Detection of Online Sexism ({EDOS}) Binary Sexism Detection (Subtask A)",
    author = "Petersen, Wiebke  and
      Tran, Diem-Ly  and
      Wroblewitz, Marion",
    editor = {Ojha, Atul Kr.  and
      Do{\u{g}}ru{\"o}z, A. Seza  and
      Da San Martino, Giovanni  and
      Tayyar Madabushi, Harish  and
      Kumar, Ritesh  and
      Sartori, Elisa},
    booktitle = "Proceedings of the 17th International Workshop on Semantic Evaluation (SemEval-2023)",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.semeval-1.203",
    doi = "10.18653/v1/2023.semeval-1.203",
    pages = "1476--1482",
    abstract = "In this paper, we describe SemEval-2023 Task 10, a shared task on detecting and predicting sexist language. The dataset consists of labeled sexist and non-sexist data targeted towards women acquired from both Reddit and Gab. We present and compare several approaches we experimented with and our final submitted model. Additional error analysis is given to recognize challenges we dealt with in our process. A total of 84 teams participated. Our model ranks 55th overall in Subtask A of the shared task.",
}
```
