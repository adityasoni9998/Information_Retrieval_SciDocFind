# SciDocFind
Information Retrieval Course Project

## Abstract
We propose an end-to-end approach for faceted scientific paper retrieval that employs the SciRepEval dataset and pre-trained language models fine-tuned with contrastive loss using triples generated from the Highly Influential Citations dataset. Experimental results demonstrate competitive performance across different facets of the CSFCube dataset and competitive performance in other facets, addressing the limitations of previous methods.

## Project Report
Please check [report.pdf](./project_report.pdf)

## Instructions for execution

- [baselines_inference.ipynb](code/baselines_inference.ipynb)
Run this notebook* to get the evaluation metrics like R-Precsion, Precision@20, and others for all the baseline models. \
A total of 7 baselines are implemented which consists of 3 abstract level baselines and 4 sentence level baselines.


- [finetune_inference.ipynb](code/finetune_inference.ipynb)
Run this notebook* after uploading CSFCube-master.zip* to get the evaluation metrics like R-Precsion, Precision@20, and others for all the fine-tuned models. Three models are finetuned - SentBERT-PP, SPECTER and SciNCL.

- [sentbert_pp_finetune.ipynb](code/sentbert_pp_finetune.ipynb)
Run this notebook** to fine-tune SentBERT-PP model using PARADE dataset.

- [specter_scincl_finetune.ipynb](code/specter_scincl_finetune.ipynb)
Run this notebook after to fine-tune SPECTER and SciNCL models using the CS papers from HIC dataset.

- [demo.ipynb](code/demo.ipynb)
Run this notebook* after uploading CSFCube-master.zip* for an interactive demo of our retrieval system.

- [SciRepEval_SciBERT_classifier.ipynb](code/SciRepEval_SciBERT_classifier.ipynb)
Run this notebook to fine-tune SciBERT model for the task of classifying the field of study of any research paper.

- \* upload [CSFCube dataset](datasets/CSFCube-master.zip) before running the notebook \
- ** upload [PARADE_dataset](datasets/PARADE_dataset-main.zip) before running the notebook
