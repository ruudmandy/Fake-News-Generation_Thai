This program will generate thai news from keywords.
to fine-tune model please run 'mt5-news-gen-th-trainning.ipynb'.

mt5-news-gen-th-trainning.ipynb will tune mT5 model by using ThaiSum
dataset by using tags to be input and summary to be label.
The process of fine-tuning  is
1) Load ThaiSum dataset.
2) Download pretrain-model from huggingface.
3) Create class ThaiSumDataset for encode.
4) Create class ThaiSumModule to load training set, validation set and test set.
5) Input tags and summary to mt5 model.
6) train mt5 model but before training, you can change parameters including batch_size, n_epoch and max_token_lenght
7) generate news for evaluation

if the results of step 7) is accepable you can push your trained model to huggingface
for application you can use 'fakenews_ui.ipynb' this program will show user interface.
