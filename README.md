# CSCI-376 Natural Language Processing Project Implementation
Created by Yuchen Wang (yw3642@nyu.edu) and Yichen Huang (yh2689@nyu.edu) in May 2021

All data, code and weights are hosted on [Kaggle](www.kaggle.com) as linked below.
## Data
- [Raw Data](https://www.kaggle.com/zacchaeus/meme-project-raw): Raw data scrapped from <memegenerator.net> including 3000 images and about 300,000 captions.
- [Cleaned Caption Data](https://www.kaggle.com/zacchaeus/meme-project-clean-json): Cleaned captions with non-English and noisy sentences removed.
## Code
- [Data Scrapper](https://www.kaggle.com/zacchaeus/meme-data): The `Python` scrapper script fetching our data from <memegenerator.net>.
- [Preprocessing](https://www.kaggle.com/zacchaeus/data-preprocess): Data pre-processing pipeline, which mainly cleans the text data.
- [Finetuning CLIP](https://www.kaggle.com/zacchaeus/clip-finetune): The pipeline for finetuning CLIP on our dataset, including both training and evaluation.
- [Finetuning BERT for Caption Splitting](https://www.kaggle.com/zacchaeus/bert-splitter): The pipeline for finetuning BERT on our dataset for caption splitting, including both training and evaluation.
## Weights
- [Finetuned CLIP Weights](https://www.kaggle.com/zacchaeus/clipfinetuneweights): The `Pytorch` weights of the finetuned CLIP model, including a `best_model.pt` which had lowest validation loss and a `last_model.pt` which overfitted the training data.
- [Fintuned BERT Weights for Caption Splitting](https://www.kaggle.com/zacchaeus/bert-splitter-dirty/settings): The `Pytorch` weights of the finetuned BERT model for caption splitting, including a `best_model.pt` which had lowest validation loss.
