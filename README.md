# ESM Secondary Structure Prediction
Fine-tuning the ESM model from HuggingFace and ensembling with gradient boost methods for secondary structure predictions

---
## Project from COM SCI C121 @ UCLA

In `ESM.ipynb`, exploratory data analysis and combining the information from `train.tsv` and `sequences.fasta` into a Pandas DataFrame were done. Then, using that DataFrame, the pre-trained ESM model from HuggingFace was loaded and fine-tuned. Additionally, different window lengths of the sequences were also tested. Predictions on the test set after fine-tuning resulted in about 60% accuracy.

In `GradBoost.ipynb`, the embeddings from the last layer of the fine-tuned ESM model were used as inputs to various gradient boosting models, such as CatBoost. Using these embeddings resulted in a slight increase in accuracy to about 65%.

`train.tsv`: https://drive.google.com/file/d/1VhJB3Uc2ZXGqFBbEFgijwRxp4elgdTud/view?usp=sharing
