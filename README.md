# TallyQA [Paper link](https://arxiv.org/abs/1810.12440)

The dataset using [this link](https://github.com/manoja328/tallyqa/blob/master/tallyqa.zip?raw=true). The zipped file contains json files for train and test respectively. Each entries in the dataset contains the following fields:
```
 {'answer': 4,
  'data_source': 'imported_genome',
  'image': 'VG_100K_2/2410408.jpg',
  'image_id': 92410408,
  'issimple': False,
  'question': 'How many headlights does the black bus have?',
  'question_id': 30095774}
```

Attributes such as *answer*, *image-id*, *image* ,*question* suggest the straighforward meanings. The boolean flag field ( **issimple**) denotes whether the question is simple (True)  or complex ( False) . The field 'data_source' shows the source of the question-answer pair. Those questios collected from AMT annotators have 'data_source' = 'amt' and likewise for other sources. The images used in the dataset are derived from COCO and Visual Genome. The imported quesiton answer pairs have been derived from [TDIUC](https://kushalkafle.com/projects/tdiuc.html) and VQA datasets.

Please cite the work using the following Bibtex:
```
@inproceedings{acharya2019tallyqa,
  title={TallyQA: Answering Complex Counting Questions},
  author={Acharya, Manoj and Kafle, Kushal and Kanan, Christopher},
  booktitle={AAAI},
  year={2019}
}

```
