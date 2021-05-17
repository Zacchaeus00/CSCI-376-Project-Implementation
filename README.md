# CSCI-376-Project-Implementation
Author: Yuchen Wang (yw3642@nyu.edu), Yichen Huang (yh2689@nyu.edu)

All data, code and weights are hosted on [Kaggle](www.kaggle.com) as linked below.
## Data
- [Raw Data](https://www.kaggle.com/zacchaeus/meme-project-raw): Raw data scrapped from <memegenerator.net> including 3000 images and about 300,000 captions.
- [Cleaned Caption Data](https://www.kaggle.com/zacchaeus/meme-project-clean-json): Cleaned captions with non-English and noisy sentences removed.
## Code
- [Preprocessing](https://www.kaggle.com/zacchaeus/data-preprocess): Data pre-processing pipeline, which mainly cleans the text data.
- [Finetuning CLIP](https://www.kaggle.com/zacchaeus/clip-finetune): The code pipeline for finetuning CLIP on our dataset, including both training and evaluation.
## Weights
- [Finetuned CLIP Wights](https://www.kaggle.com/zacchaeus/clipfinetuneweights): The `Pytorch` weights of the finetuned CLIP model, including a `best_model.pt` which had lowest validation loss and a `last_model.pt` which overfitted the training data.
