# Modern EgyBert - Egyptian Arabic Fine-Tuned BERT Model

Modern EgyBert is a 🤗 Transformers-based **BERT** model fine-tuned specifically for **Egyptian Arabic**, leveraging the **FineWeb2** dataset. It is built upon **Modern Bert Base** and optimized for downstream **Natural Language Processing (NLP)** tasks involving Egyptian Arabic.

## 🚀 Model Overview

- **Model Name**: Modern EgyBert
- **Base Model**: Modern Bert Base
- **Dataset**: Egyptian Arabic split of **FineWeb2**
- **Languages**: Egyptian Arabic 🇪🇬
- **Frameworks**: 🤗 Transformers, PyTorch

### 🎯 Evaluation Metrics
The model achieved the following results on the evaluation set:

| Metric                     | Value  |
|----------------------------|--------|
| **Eval Loss**              | 2.5126 |
| **Eval Runtime**           | 134.99s |
| **Eval Samples/Sec**       | 68.267 |
| **Eval Steps/Sec**         | 8.533 |
| **Epochs**                 | 3 |
| **Total Training Steps**   | 120000 |

## 🛠️ Training Details

### **Training Hyperparameters**
- **Learning Rate**: `5e-5`
- **Train Batch Size**: `32`
- **Eval Batch Size**: `8`
- **Seed**: `42`
- **Optimizer**: AdamW (`betas=(0.9,0.999)`, `epsilon=1e-08`)
- **Learning Rate Scheduler**: Linear (`warmup_steps=500`)
- **Number of Epochs**: `3`

### **Frameworks & Libraries**
- 🤗 **Transformers**: `4.49.0.dev0`
- 🔥 **PyTorch**: `2.5.1+cu124`
- 📚 **Datasets**: `3.2.0`
- ✂ **Tokenizers**: `0.21.0`

---

## 📦 Installation

Before using the model, make sure you have the necessary dependencies installed:

```bash
pip install torch transformers datasets tokenizers
