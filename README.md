# TallyQA https://arxiv.org/abs/1810.12440

The dataset can be downloaded from  https://github.com/manoja328/tallyqa/blob/master/tallyqa.zip?raw=true. The zip contains json files for train and test respectively. Each entries in the dataset contains the following fields:
```
 {'answer': 4,
  'data_source': 'imported_genome',
  'image': 'VG_100K_2/2410408.jpg',
  'image_id': 92410408,
  'issimple': False,
  'question': 'How many headlights does the black bus have?',
  'question_id': 30095774}
```

Fileds such as answer, image-id , image are as the name suggest. Besides, there is also  a flag ( **issimple**) to denote 
whether the question is simple or complex, and  the field 'data_source' shows the source of the question-answer pair. All the images are from COCO and Visual Genome. The quesiton answer pairs have been derived from TDIUC, VQA2.0 and also using AMT annotators.
