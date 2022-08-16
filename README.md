
# Self-Teaching Machines to Read and Comprehend with Large-Scale Multi-Subject Question-Answering Data


## Overview

This repository maintains the resource ExamQA for the above EMNLP'21 (Findings) paper. Please contact examqa@dataset.org if you have any questions or suggestions.

[Paper](https://aclanthology.org/2021.findings-emnlp.6/):
```
@inproceedings{yu-2021-self-teaching,
    title = "Self-Teaching Machines to Read and Comprehend with Large-Scale Multi-Subject Question-Answering Data",
    author = "Yu, Dian  and
      Sun, Kai  and
      Yu, Dong  and
      Cardie, Claire",
    booktitle = "Findings of the EMNLP 2021",
    year = "2021",
    address = "Punta Cana, Dominican Republic",
    url = "https://aclanthology.org/2021.findings-emnlp.6",
    pages = "56--68"
}
```

## Data

Data file in this repository:

* ```wiki_all.json```: 638.4K Chinese multiple-choice machine reading comprehension (MRC) instances in which the documents are noisy snippets retrieved from Wikipedia. This can be used to augment data for both extractive and multiple-choice MRC tasks. The ExamQA dataset can be downloaded from [Weiyun](https://share.weiyun.com/VM4UpT0Z).


* The format is as follows:
```
[
  [
    [
      document 1
    ],
    [
      {
        "question": document 1 / question 1,
        "choice": [
          document 1 / question 1 / answer option 1,
          document 1 / question 1 / answer option 2,
          document 1 / question 1 / answer option 3,
          document 1 / question 1 / answer option 4
        ],
        "answer": document 1 / question 1 / correct answer option
      }
    ],
    document 1 / question 1 / id
  ],
  ...
]
```



## Fine-Tuning
Please refer to [SCRIPT](https://github.com/nlpdata/script) for the hard-label or soft-label fine-tuning code.


## Disclaimer
This is not an officially supported Tencent product.




