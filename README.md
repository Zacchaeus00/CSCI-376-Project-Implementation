# Meme Caption Generation
This is the implementation of our course project in CSCI-376 Natural Language Processing taught by [Prof. Yik-Cheung Tam](https://shanghai.nyu.edu/academics/faculty/directory/yik-cheung-wilson-tam) at NYU Shanghai.
*Yuchen Wang (yw3642@nyu.edu)* and *Yichen Huang (yh2689@nyu.edu)*, May 2021.

## Paper Report
[report(pdf)](https://github.com/Zacchaeus14/CSCI-376-Project-Implementation/blob/main/nlp_final_report.pdf?raw=true)   
[presentation slides](https://docs.google.com/presentation/d/1vRHRJ6RL9uaqlVlzu8dMmI7Kb7LRWh64vFyEQHotFi0/edit?usp=sharing)

## Pipeline Architecture
![pipeline architecture](https://github.com/Zacchaeus14/CSCI-376-Project-Implementation/blob/main/model_diagram.png?raw=true "pipeline architecture")

## Example Output
![sample model outputs](https://cdn.shanghai.nyu.edu/sites/default/files/media/screen_shot_2021-09-29_at_11.31.00_pm.png "sample model outputs")

## Data
- [Raw Data](https://www.kaggle.com/zacchaeus/meme-project-raw): Raw data scrapped from [memegenerator.net](www.memegenerator.net) including 3000 images and about 300,000 captions.
- [Cleaned Caption Data](https://www.kaggle.com/zacchaeus/meme-project-clean-json): Cleaned captions with non-English and noisy sentences removed.
## Code
### Data and Preprocessing
- [Data Scrapper](https://www.kaggle.com/zacchaeus/meme-data): The `Python` scrapper script fetching our data from [memegenerator.net](www.memegenerator.net).
- [Preprocessing](https://www.kaggle.com/zacchaeus/data-preprocess): Data pre-processing pipeline, which mainly cleans the text data.
### Main Pipeline
Both of these notebooks contain everything from data loading to evaluation and can be run independently. Note that we do not include the BERT splitter in the main pipeline.
- [Baseline](https://www.kaggle.com/ineed21eep/meme-baseline-final): The baseline pipeline using a standard encoder-decoder. 
- [Proposed](https://www.kaggle.com/winogradtamson/meme-variation-final): The proposed pipeline with naive / MMI / CLIP score decoding. 
### Pipeline Components
- [Finetuning CLIP](https://www.kaggle.com/zacchaeus/clip-finetune): The pipeline for finetuning CLIP on our dataset, including both training and evaluation.
- [Finetuning BERT for Caption Splitting](https://www.kaggle.com/zacchaeus/bert-splitter): The pipeline for finetuning BERT on our dataset for caption splitting, including both training and evaluation.
## Model Weights
- [Weights and dataloaders for the baseline encoder-decoder](https://www.kaggle.com/theotherotherwill/baseline-best): The `PyTorch` weights of the baseline encoder-decoder. Comes with the validation and test loaders used in training and evaluation.
- [Weights and dataloaders for the proposed encoder-decoder](https://www.kaggle.com/theotherotherwill/variation-best): The `PyTorch` weights of the proposed encoder-decoder. Comes with the validation and test loaders used in training and evaluation.
- [Finetuned CLIP Weights for Image-Caption Matching](https://www.kaggle.com/zacchaeus/clipfinetuneweights): The `PyTorch` weights of the finetuned CLIP model, including a `best_model.pt` which had lowest validation loss and a `last_model.pt` which overfitted the training data.
- [Fintuned BERT Weights for Caption Splitting](https://www.kaggle.com/zacchaeus/bert-splitter-dirty/settings): The `PyTorch` weights of the finetuned BERT model for caption splitting, including a `best_model.pt` which had lowest validation loss.
