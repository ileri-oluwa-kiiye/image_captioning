# Image Captioning with Visual Attention

This repository contains an end-to-end implementation of an **image captioning model with attention**, trained on the **Flickr8k dataset**. The project is based on the [Image Captioning with Visual Attention](https://www.cloudskillsboost.google/course_templates/542) course by Google Cloud Skills Boost, and follows the **Show, Attend and Tell** architecture.

---

## Files in This Repo

- `flickr-captioning.ipynb`: The main notebook for preprocessing, training, and saving the attention-based captioning model.
- `caption_predictions.csv`: CSV file containing generated captions for test images.

---

## Project Overview

This project uses an encoder-decoder model with attention to generate descriptive captions for images:

- **Encoder**: A pretrained CNN (e.g., InceptionV3) extracts spatial features from images.
- **Attention Layer**: Learns where to "look" in the image at each decoding step.
- **Decoder**: An LSTM generates captions word by word based on attended features.

---

## 📊 Dataset

The [Flickr8k Dataset](https://www.kaggle.com/datasets/adityajn105/flickr8k), which contains:

- 8,000+ images
- 5 human-annotated captions per image
