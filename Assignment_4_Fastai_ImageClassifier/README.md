# Assignment 4 — Image Classification with Fastai (Brain Tumor Dataset)

In this assignment, we build and fine-tune a convolutional neural network (CNN) using the `fastai` library. The model is trained on a custom brain MRI dataset to classify images into four categories of brain tumors — or detect the absence of one.

---

## 🧠 Objective

To fine-tune a pre-trained image classification model (ResNet34) using Fastai on a 4-class dataset containing:
- Glioma
- Meningioma
- Pituitary Tumor
- No Tumor

---

## ⚙️ Tools & Libraries

| Library       | Purpose                            |
|---------------|------------------------------------|
| 🧠 `fastai`    | Model training, augmentation, metrics |
| 🖼️ `PIL`        | Image loading and preprocessing   |
| 📊 `matplotlib`| Visualization (confusion matrix, top losses) |
| 🗂️ `shutil`     | Organizing Training & Testing images |

---

## 🧪 Model Details

| Setting       | Value               |
|---------------|---------------------|
| Model         | ResNet34 (pretrained) |
| Image Size    | 224x224              |
| Epochs        | 4                    |
| Optimizer     | Adam (default in Fastai) |
| Validation Split | 20%               |

---

## 📂 Project Structure

- `Fastai_HW.ipynb` — Notebook with full training and evaluation pipeline
- `README.md` — This documentation
- Dataset (locally structured as `Training/` and `Testing/`, later combined)

---

## 📊 Evaluation

- 📈 Accuracy score
- 📉 Confusion matrix
- ❌ Top misclassifications (via `plot_top_losses`)

> 💡 These metrics help visualize model strengths and weaknesses.

---

## 🧪 Sample Code Snippet

'''python

learn = cnn_learner(dls, resnet34, metrics=accuracy)
learn.fine_tune(4)
interp = ClassificationInterpretation.from_learner(learn)
interp.plot_confusion_matrix()
interp.plot_top_losses(6, nrows=2)
