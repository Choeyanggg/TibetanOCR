# TibetanOCR

TibetanOCR is an Optical Character Recognition (OCR) system built to transcribe Tibetan script from line images into digital text. It leverages PyTorch and HuggingFace's Transformers and Datasets libraries, utilizing a dataset curated by Monlam AI Lab. The model is designed to run efficiently in Google Colab with GPU support.

---

## Features

- OCR for **Tibetan script** from line-level image data  
- Based on **transformer models** and tokenization with HuggingFace  
- Trained on [MonlamAI's OCR-Tibetan dataset](https://huggingface.co/datasets/MonlamAI/OCR-Tibetan_line_to_text_benchmark)  
- Built-in support for **Google Colab** and **Google Drive** for data and checkpoint storage  
- Custom PyTorch `Dataset` class and dynamic image preprocessing pipeline

---

## Prerequisites

- Python 3.8+
- PyTorch >= 1.10
- Transformers
- Datasets (from HuggingFace)
- Torchvision
- PIL, OpenCV, NumPy, Pandas
- Google Colab (preferred for training with GPU)

---

## Model Architecture

- CNN + Transformer encoder-decoder
- Custom attention masks and padding strategies
- **Loss**: `CrossEntropyLoss`
- **Optimizer**: `Adam`
