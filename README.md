# Fine-Tuning Llama 2 Using QLoRA

QLoRA (Quantization Low-Rank Adaptation) is an efficient method for fine-tuning large language models like Llama 2. It combines quantization techniques with low-rank adaptation to reduce memory usage while maintaining performance.

---

## Table of Contents

1. [Setup Environment](#setup-environment)
2. [Prepare Dataset](#prepare-dataset)
3. [Fine-Tuning with QLoRA](#fine-tuning-with-qlora)
4. [Save and Evaluate Model](#save-and-evaluate-model)

---


Before starting, ensure you have the following:

- Python 3.9 or higher
- NVIDIA GPU with CUDA support
- Hugging Face `transformers` and `peft` libraries installed
- Access to the Llama 2 model weights (via Hugging Face Hub)

---


Install the required libraries by running the following commands:

```bash
pip install -q accelerate==0.21.0 peft==0.4.0 bitsandbytes==0.40.2 transformers==4.31.0 trl==0.4.7
