# TallyQA - [ AAAI 2019 Paper link](https://arxiv.org/abs/1810.12440)
## Project page - https://www.manojacharya.com/tallyqa.html
## UPDATE: Code available at https://github.com/manoja328/tallyqacode

## TallyQA Stats
TallyQA is the only dataset to distinguish between simple and complex counting questions. Moreover, to make sure that the complex questions have conterfactuals in images, we use Amazon Mechanical Turk (AMT) for data collection. In summary, it has
- 287K questions
- 165K images
- 19K complex questions collected from human annotators using AMT

## Download QA pairs
Please, download the dataset using [this link](https://github.com/manoja328/tallyqa/blob/master/tallyqa.zip?raw=true). The zipped file contains json files for train and test splits. Each entries in the dataset contains the following fields:
```
 {'answer': 4,
  'data_source': 'imported_genome',
  'image': 'VG_100K_2/2410408.jpg',
  'image_id': 92410408,
  'issimple': False,
  'question': 'How many headlights does the black bus have?',
  'question_id': 30095774}
```

Attributes such as `answer, image_id, image ,question` should be straighforward. The  `issimple` boolean flag field  denotes whether the question is simple (True) or complex ( False). The  `data_source` field shows the source of the question-answer pair. Questions collected from AMT annotators have `data_source = amt`. The imported QA pairs are derived/filtered from [TDIUC](https://kushalkafle.com/projects/tdiuc.html) and [VQA](https://visualqa.org/) datasets.

## Download Images
The images used in the dataset are derived from [COCO](http://cocodataset.org/) and [Visual Genome](https://visualgenome.org/). All the images can be downloaded from the publicly available datasets below:
* https://homes.cs.washington.edu/~ranjay/visualgenome/api.html (Visual Genome dataset)
* https://visualqa.org/download.html (COCO train/val images)
* HowmanyQA dataset can be downloaded from this repo or follow the setup instructions from [HowmanyQA](https://github.com/sanyam5/irlc-vqa-counting/blob/master/tools/download_hmqa.sh )

Please cite the work using the following Bibtex:
```
@inproceedings{acharya2019tallyqa,
  title={TallyQA: Answering Complex Counting Questions},
  author={Acharya, Manoj and Kafle, Kushal and Kanan, Christopher},
  booktitle={AAAI},
  year={2019}
}

```
