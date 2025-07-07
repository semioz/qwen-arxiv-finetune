# qwen-arxiv-finetune

## **Project Overview**
Fine-tuning a pre-trained model on the **arXiv Machine Learning Papers dataset**. The goal is to enable the model to summarize and generate responses to technical research topics in machine learning and artificial intelligence. This is achieved using **Low-Rank Adaptation (LoRA)** for efficient fine-tuning and **4-bit quantization** to optimize memory usage for large models.

The trained model is on Hugging Face Hub:
**[semihb/Qwen-3-32B-ML-Expert-Reasoning](https://huggingface.co/semihb/Qwen-3-32B-ML-Expert-Reasoning)**

---

## **Technologies**
- **Model**: `Qwen-3-32B`
- **Tokenizer**: Hugging Face `AutoTokenizer`
- **Training Framework**: Hugging Face `Trainer`, **LoRA**, **DataCollatorForLanguageModeling**
- **Quantization**: `BitsAndBytesConfig` for 4-bit quantization
- **Platform**: **RunPod**
- **Deep Learning Framework**: **PyTorch** with `torch.bfloat16` precision for training
- **Dataset**: `CShorten/ML-ArXiv-Papers` from Hugging Face Datasets