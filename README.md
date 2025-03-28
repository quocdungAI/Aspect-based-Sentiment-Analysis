## Aspect-Based Sentiment Analysis

### Introduction
The **Aspect-Based Sentiment Analysis** project aims to address the problem of sentiment analysis based on specific aspects in product or service reviews. For example, given the sentence:

> *"The price was too high, but the cab was amazing."*

The system extracts aspects like `price` and `cab`, along with their corresponding sentiment (**negative** for `price` and **positive** for `cab`).

This project consists of the following sub-tasks:

- **Aspect Term Extraction (ATE)**: Extracting the aspects mentioned in the reviews.
- **Aspect Term Sentiment Classification (ATSC)**: Predicting the sentiment of each aspect based on the input text.

---

## Project Content
The project is built in two main steps:

### Dataset
Dataset used: [ABTE-Restaurants](https://huggingface.co/datasets/thainq107/abte-restaurants)

---

## Step 1: Aspect Term Extraction (ATE)

![ATE Diagram](https://github.com/user-attachments/assets/2f53f85b-a781-4b50-95c1-c8cd0c899a91)

### Preprocessing
- Removing punctuation
- Normalizing text
- Tokenizing by whitespace

### Model
- Utilizing **sequence labeling** with the **DistilBERT** pre-trained model

### Results
- Accuracy on the test set: **81.73%**

---

## Step 2: Aspect Term Sentiment Classification (ATSC)
![image](https://github.com/user-attachments/assets/4b2d4056-3f8b-4451-af0a-ca9811977129)

### Model
- Building a sentiment classification model for each aspect using **DistilBERT**

### Results
- Accuracy on the test set: **79.18%**
