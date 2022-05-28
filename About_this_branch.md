# About the Data

* The data was taken from https://www.finra.org/rules-guidance/key-topics 

* The Data consist of three columns: Rule, Text and Topic.
  - Rule: FINRA Rule number. 
  - Text: List of rules.
  - Topic: Category to which the rule belongs.

* Each rule under the Key Topics: <br>

  1. Anti-Money Laundering
  2. Broker-Dealer Recruitment Disclosures: Complying with FINRA Rule 2273
  3. Business Continuity Planning
  4. Electronic Blue Sheets 
  5. Senior Investors
  6. Subordination Agreements 

are taken as a text.

* The rules are summarized with no duplicate text and the character count is not more than 512.
* Blank text is not considered.
* Prefixes in the beginning of the rules are removed.
* The word ‘and’ to indicate the last rule is removed.
* All sentences are considered.

# Text Preprocessing

* Duplicate ‘Text’ if any are removed.

The notebook containing the pre-processing of input 'Text' is **Part1_HuggingFace_Dataset.ipynb**

The notebooks containing the fine-tuning of DistilBERT model for 50 epochs are:

1.  **Part2_DistilBERT_50_epochs**
2.  **Part3_DistilBERT_Predicting_and_Inference_using_Pipeline_50_epochs.ipynb**

The notebooks containing the fine-tuning of BERT model for 50 epochs are:

1.  **Part2_BERT_50_epochs**
2.  **Part3_BERT_Predicting_and_Inference_using_Pipeline_50_epochs.ipynb**
