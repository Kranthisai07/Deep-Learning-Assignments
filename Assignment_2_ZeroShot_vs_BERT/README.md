# Assignment 2 — Zero-Shot vs Fine-Tuned BERT Classifier

In this assignment, we compare the performance of two powerful NLP approaches for text classification:

1. **Zero-Shot Classification** using `roberta-large-mnli`
2. **Fine-Tuned BERT** classifier trained on the same dataset

---

## 🧠 Objective

To determine which model performs better under the same evaluation setup, and understand trade-offs between:
- Pre-trained zero-shot models (no additional training)
- Fine-tuned BERT models (trained specifically for the task)

---

## ⚙️ Tools & Libraries

| Library | Purpose |
|--------|---------|
| 🤗 `transformers` | Access to `pipeline`, `BertForSequenceClassification`, etc. |
| 📊 `sklearn` | Metrics like accuracy, F1 score, confusion matrix |
| 🧪 `pandas` & `numpy` | Data processing and manipulation |

---

## 🧪 Models Compared

| Model Type         | Model Used             | Notes |
|--------------------|------------------------|-------|
| Zero-Shot          | `roberta-large-mnli`   | Performs inference without training |
| Fine-Tuned BERT    | `bert-base-uncased`    | Fine-tuned on labeled dataset |

---

## 📊 Metrics Reported

- **Accuracy**
- **F1 Score**
- **Precision / Recall**
- **Confusion Matrix**

_(Include a table or screenshot if possible)_

---

## 📂 Project Structure

- `ZeroShotandBert.ipynb` — Full comparison notebook
- `README.md` — This documentation

---

## 🔍 Observations

- Zero-shot classification performs surprisingly well on generic topics.
- Fine-tuned BERT achieves **higher accuracy** when trained on domain-specific data.
- Trade-off: Fine-tuning needs data + time, but offers better performance on specific tasks.

---

## 💡 Future Work

- Compare with larger models like `bert-large` or `deberta`
- Test zero-shot classification using `facebook/bart-large-mnli`
- Apply to real-world domain data (e.g., news, legal, or healthcare)

---

## 📌 Status

✅ Model pipelines implemented  
✅ Evaluation and comparison completed  
✅ Conclusions drawn based on metrics

---

## 📜 License

This project is for academic use under the Deep Learning Spring 2025 course.
