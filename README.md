# Fact Finders

Welcome to the Fact Finders NLP task repository. This repository contains all the necessary files and folders to train and test NLP models for generating predictions in multiple languages. Below is an overview of the folder structure and how to use the provided codes to reproduce the results.

## Folder Structure

Fact Finders/
│
├── additional_dataset/
│ └── ... (additional dataset files)
│
├── Codes/
│ ├── 1. Train-Ensemble.py
│ ├── 1. Train.py
│ ├── 2. Test-Ensemble.py
│ ├── 2. Test.py
│
├── preds/
│ ├── hi_0.json
│ ├── hi_1.json
│ ├── en_0.json
│ ├── en_1.json
│ ├── ml_0.json
│
├── readme.md
├── requirements.txt
└── report.pdf


## Installation

To run the provided codes, you need to install the required dependencies. Use the following command to install the dependencies listed in `requirements.txt`:

```sh
pip install -r requirements.txt

Usage
Training Models
Pure Models
To train a pure model and generate predictions (e.g., hi_0.json, en_0.json, ml_0.json), edit the 1. Train.py file to include the model ID and path location at the beginning of the code. Then run the script using:

sh
Copy code
python Codes/1. Train.py
Ensemble Models
To train an ensemble model and generate predictions (e.g., hi_1.json, en_1.json), edit the 1. Train-Ensemble.py file to include the model IDs and path locations at the beginning of the code. Then run the script using:

sh
Copy code
python Codes/1. Train-Ensemble.py
Testing Models
Pure Models
To test a pure model and validate predictions, run:

sh
Copy code
python Codes/2. Test.py
Ensemble Models
To test an ensemble model and validate predictions, run:

sh
Copy code
python Codes/2. Test-Ensemble.py
Model Information
Pure Models
English: DeBerta-Large
Hindi: Muril-Base
Multi-Lingual: DeBerta-Large
Ensemble Models
English
DeBerta-Large
Distil-BERT
RoBERTa-Base
Hindi
Muril-Base
XLM-R Large
Multi-Lingual BERT
Multi-Lingual
Ensemble models were not performed for multi-lingual tasks.

Predictions
hi_0.json: Predictions for the pure Hindi model.
hi_1.json: Predictions for the ensemble Hindi model.
en_0.json: Predictions for the pure English model.
en_1.json: Predictions for the ensemble English model.
ml_0.json: Predictions for the pure Multi-Lingual model.
Additional Information
For detailed information about the project, refer to the report.pdf file in the root directory.

