# ClassActionPrediction

## Paper 

[ClassActionPrediction: A Challenging Benchmark for Legal Judgment Prediction of Class Action Cases in the US](https://arxiv.org/abs/2211.00582). Gil Semo, Dor Bernsohn, Ben Hagag, Gila Hayat and Joel Niklaus. 2022.

The research field of Legal Natural Language Processing (NLP) has been very active recently, with Legal Judgment Prediction (LJP) becoming one of the most extensively studied tasks. To date, most publicly released LJP datasets originate from countries with civil law. In this work, we release, for the first time, a challenging LJP dataset focused on class action cases in the US. It is the first dataset in the common law system that focuses on the harder and more realistic task involving the complaints as input instead of the often used facts summary written by the court. Additionally, we study the difficulty of the task by collecting expert human predictions, showing that even human experts can only reach 53% accuracy on this dataset. Our Longformer model clearly outperforms the human baseline (63%), despite only considering the first 2,048 tokens. Furthermore, we perform a detailed error analysis and find that the Longformer model is significantly better calibrated than the human experts. Finally, we publicly release the dataset and the code used for the experiments.



## Dataset 
USClassActions is an English dataset of 3K complaints from the US Federal Court with the respective binarized judgment outcome (Win/Lose). The dataset poses a challenging text classification task. We are happy to share this dataset in order to promote robustness and fairness studies on the critical area of legal NLP.

[Hugging Face Dataset](https://huggingface.co/datasets/darrow-ai/USClassActions).

## Requirements
```
transformers>==4.17.0
torch==1.11.0+cu113
tokenizers==0.12.1
spacy==3.2.3
scikit-learn==1.1.1
pandas==1.3.4
numpy==1.20.3
netcal==1.2.1
nltk==3.6.5
matplotlib==3.4.3
```
## Citations 
If you use our work in your research, please cite:

[ClassActionPrediction: A Challenging Benchmark for Legal Judgment Prediction of Class Action Cases in the US](https://arxiv.org/abs/2211.00582). Gil Semo, Dor Bernsohn, Ben Hagag, Gila Hayat and Joel Niklaus. 2022. arXiv:2211.00582 .

```
@misc{chalkidis-etal-2022-hat,
  url = {https://arxiv.org/abs/2211.00582},
  author = {Semo, Gil and Bernsohn, Dor and Hagag, Ben and Hayat, Gila and Niklaus, Joel},
  title = {ClassActionPrediction: A Challenging Benchmark for Legal Judgment Prediction of Class Action Cases in the US},
  publisher = {arXiv},
  year = {2022},
}
```

