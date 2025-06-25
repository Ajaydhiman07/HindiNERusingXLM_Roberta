# Hindi-NER-XLM-RoBERTa

This project fine-tunes the multilingual transformer model **XLM-RoBERTa** for **Named Entity Recognition (NER)** in **Hindi** using the [`cfilt/HiNER-original`](https://huggingface.co/datasets/cfilt/HiNER-original) dataset.

It leverages the Hugging Face Transformers and Datasets libraries to tokenize, align labels, train, evaluate, and test the model. Final inference is done using the `pipeline("ner")`.

---

## 🚀 Features

- Fine-tunes `xlm-roberta-base` on HiNER dataset  
- Computes evaluation metrics: **precision**, **recall**, **f1**, and **accuracy**  
- Uses Hugging Face `Trainer` API  
- Inference demo using Hindi sentence  
- Output available in Jupyter Notebook with results  

---

## 📁 Files

- `HindiNERusingRobertaFinal.ipynb` — Full notebook with training + inference

---

## 🛠️ Libraries Used

- `transformers`
- `datasets`
- `evaluate` (for `seqeval`)
- `pandas`
- Hugging Face Hub

---

## 📝 Dataset

- **Name**: `cfilt/HiNER-original`
- **Language**: Hindi
- **Labels**: `PER`, `LOC`, `ORG`, `MISC`, etc. (**23 total**)

---

## 📈 Model

- **Base model**: `xlm-roberta-base`
- Fine-tuned for **token classification**

---

## 📦 Run Locally (Optional)

```bash
pip install transformers datasets accelerate evaluate seqeval
