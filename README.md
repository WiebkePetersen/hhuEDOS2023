# hhuEDOS2023

This repository contains the source code for the models used for hhuEDOS team's submission for <a href="https://codalab.lisn.upsaclay.fr/competitions/7124" target="_blank">SemEval-2023 Shared Task 10, Subtask A “Explainable Detection of Online Sexism (EDOS)"</a>. We ranked 55th out of 84 teams.



## Overview

Listed below are all our methods we experimented with. Our submitted model (notebook 3) uses semi-supervised learning and yieled results with a macro F1 score of 81.85%. 

| Notebook | Description |
| ------------- | ------------- |
| Task_EDOS_Semeval_0_baseline  | Content Cell  |
| Task_EDOS_Semeval_1_imbalanced_data | Content Cell  |
| Task_EDOS_Semeval_2_semi-supervised | Apply our pretrained language model on additional unlabeled data to augment the dataset and re-train the model.|
| Task_EDOS_Semeval_3_ML | Apply traditional machine learning methods and test several classifiers with different parameter settings. Features are extracted using TF-IDF.|

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


