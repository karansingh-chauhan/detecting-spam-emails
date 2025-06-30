# 📧 Spam Email Detection using TensorFlow
detecting-spam-emails-using-tensorflow-in-python

This project is a machine learning-based email classifier that uses **LSTM** (Long Short-Term Memory) neural networks to distinguish between **Spam** and **Ham** (not spam) emails. Built with Python, TensorFlow, and various NLP tools.
# 📥 How to Use a CSV File from GitHub in Google Colab

This guide explains how to:

1. Download a `.csv` file from a GitHub repository
2. Save it to your local desktop
3. Upload it into Google Colab
4. Load and browse it using `pandas`

---

## 📁 Step 1: Download CSV from GitHub

1. Go to the GitHub repository that contains the CSV file (e.g., `Emails.csv`)
2. Click on the CSV file
3. Click the **"Download raw"** button or **"Raw"** button on the file page
4. Press **`Ctrl + S`** or **right-click → Save As**
5. Save the file to a known location on your desktop (e.g., `Downloads` or `Desktop`)

✅ Make sure the file is saved with a `.csv` extension.

---

## 🧭 Step 2: Open Google Colab

1. Visit [https://colab.research.google.com](https://colab.research.google.com)
2. Create a new notebook (File → New notebook)

---

## ⬆️ Step 3: Upload the CSV File from Desktop to Colab

Paste the following code in a cell:

```python
from google.colab import files
uploaded = files.upload()


## 📂 Dataset

The model expects a `.csv` file with the following structure:

| label | text         |
|-------|--------------|
| ham   | Email text...|
| spam  | Email text...|

You can use the [`Emails.csv`](#) file or upload your own dataset.

---

## 🚀 Features

- Preprocesses email text (removes punctuation and stopwords)
- Balances the dataset
- Visualizes word frequencies using word clouds
- Converts text to sequences using Keras Tokenizer
- Builds and trains an LSTM model
- Predicts whether a custom email is spam or not

---

## 📁 How to Use in Google Colab

### 1️⃣ Upload CSV File from Desktop

Paste this in a code cell:

```python
from google.colab import files
uploaded = files.upload()
