# 🐕 Dog Vision – Multi-Class Dog Breed Classification

This project builds an **end-to-end multi-class image classifier** to classify dog breeds using **TensorFlow 2.x** and **TensorFlow Hub**.

---

## 🚩 1. Problem Statement

Given an image of a dog, the goal is to **identify its breed**.

> For example, you're sitting at a café, spot a cute dog, take a photo of it — and you want to know what breed it is.

---

## 📂 2. Data

- The data is from the **Kaggle Dog Breed Identification** competition.
- It consists of images labeled by breed (train set) and unlabeled images (test set).

### Dataset Overview

- 🐶 120 different dog breeds
- 🖼️ 10,000+ labeled training images
- 🖼️ 10,000+ unlabeled test images

---

## 🎯 3. Evaluation Metric

The evaluation is based on:
- A **CSV file** containing the **prediction probabilities** for each dog breed, for each test image.
- For example:

id,affenpinscher,afghan_hound,...,yorkshire_terrier
000621fb3cbb32d8935728e48679680e,0.0007,0.0002,...,0.0012


---

## 🧠 4. Features and Approach

- 🧱 **Image Classification Task** using **Deep Learning**
- ⚙️ Leveraging **Transfer Learning** with models from **TensorFlow Hub**
- 🧪 Data Preprocessing includes:
  - Reading image paths and labels
  - Converting images into tensors
  - Normalizing and resizing input
- 🧰 Model built and trained using:
  - `tf.keras`
  - `tf.data.Dataset` pipeline
  - `MobileNetV2` or similar architecture

---
