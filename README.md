# 🎨 AI Doodle Sketch Classifier

An interactive deep learning web app that allows users to draw sketches on a canvas, and the model predicts what the sketch is (e.g., cat, tree, fish, etc.).

---

## 🚀 Features

- 🖌️ Real-time drawing canvas
- 🧠 CNN-based sketch classifier using QuickDraw dataset
- 📊 Visualizes model predictions interactively
- 💻 Web app interface using Streamlit (in development)
- 🌐 Live demo (in development)

---

## 🧰 Tech Stack

| Component      | Tool              |
|----------------|-------------------|
| Language       | Python            |
| Data           | QuickDraw Dataset |
| Model          | CNN (Keras)       |
| UI             | Jupyter / Streamlit |
| Deployment     | Streamlit Cloud / Hugging Face Spaces |

---

## 📁 Dataset Info

This project uses the [QuickDraw Dataset](https://github.com/googlecreativelab/quickdraw-dataset) by Google.  
To keep this repository lightweight and within GitHub's file size limits, **the dataset files (`.npy`) are not uploaded to the repo**.

### 🔸 Classes Used:
- `cat`
- `fish`
- `ice_cream`
- `swan`
- `tree`

Each class file contains ~138,000 28x28 grayscale sketches in NumPy `.npy` format.

### 📥 How to Set Up the Dataset:

1. Download class `.npy` files from the official bucket:  
   👉 https://console.cloud.google.com/storage/browser/quickdraw_dataset/full/numpy_bitmap

2. Place them inside the following directory: `/dataset/`

3. The project expects files named:

- dataset/cat.npy
- dataset/fish.npy
- dataset/ice_cream.npy
- dataset/swan.npy
- dataset/tree.npy


4. Don't forget to install dependencies:
```bash
pip install numpy matplotlib
