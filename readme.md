# HAF Model
- A Tensorflow implementation of [Hierarchical Attention Flow for
Multiple-Choice Reading Comprehension](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/viewFile/16331/16177).
- Specially designed for [oqmrc](https://pan.baidu.com/s/1W5yCTbSxxR1IyHctGlamuw)(password:duco) dataset.
- Project is based on [a R-Net implementation](https://github.com/HKUST-KnowComp/R-Net).
# Requirements
- Python = 3.6.0
- Tensorflow-gpu = 1.5.0
- spaCy >= 2.0.0
- tqdm
# Getting started
## Download dataset
Download dataset from [oqmrc](https://pan.baidu.com/s/1W5yCTbSxxR1IyHctGlamuw)(password:duco), and unzip downloaded files.Remember to modify your data path before training.
## Download Chinese word vector
- A pre-training word vector is required, for Chinese word vectors you can refer to [here](https://github.com/Embedding/Chinese-Word-Vectors).
- We utilized [Zhihu_QA](https://pan.baidu.com/s/1VGOs0RH7DXE5vRrtw6boQA) word vectors in our experiments.
## Preprocessing
`python config --mode prepro`
## Train
`python config --mode train`
## predict
`python config --mode test`
# Result
Single-model accuracy on dev set is 0.7287.
