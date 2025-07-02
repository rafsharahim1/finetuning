# 🦙 TinyLLaMA Fine-Tuning: Supervised + Preference Alignment

This project showcases a full fine-tuning pipeline for **TinyLLaMA**, a compact decoder-only language model. Our objective was to make this lightweight model **more helpful, safe, and instruction-aligned** using a **two-stage process**:

1. **Supervised Fine-Tuning (SFT)** with LoRA for instruction-following behavior.
2. **Direct Preference Optimization (DPO)** for safety, refusal, and ethical alignment.

> 📘 A detailed research-style report of this project is available in the repo.

---

## 🧠 Project Highlights

- ✅ Instruction tuning with [`databricks-dolly-15k`](https://huggingface.co/datasets/databricks/databricks-dolly-15k)
- ✅ Preference alignment with [`PKU-SafeRLHF`](https://huggingface.co/datasets/PKU-Alignment/PKU-SafeRLHF)
- ✅ Efficient fine-tuning using LoRA (Low-Rank Adaptation)
- ✅ Experiments across **7 SFT trials** and **5 DPO trials**
- ✅ Evaluation via **BLEU scores** and **manual prompt assessments**
- ✅ Interactive Streamlit-based demo UI

---

## 📦 Features

| Phase | Technique | Goal |
|-------|-----------|------|
| **SFT** | LoRA + Instruction Dataset | Teach model to follow instructions accurately |
| **DPO** | Human Preference Dataset | Align model to be safe, helpful, and ethically grounded |
| **Frontend** | Streamlit + LocalTunnel | Demo the model and manually test responses |

---

## 🧰 Tech Stack

- Python 3.10
- Hugging Face Transformers, Datasets, PEFT, TRL
- LoRA (for efficient parameter tuning)
- Streamlit (for app interface)
- Google Colab & Kaggle GPUs (NVIDIA T4)
- Evaluation: BLEU Score + Manual Judgment

---

## 📁 Directory Structure

# 🦙 TinyLLaMA Fine-Tuning: Supervised + Preference Alignment

This project showcases a full fine-tuning pipeline for **TinyLLaMA**, a compact decoder-only language model. Our objective was to make this lightweight model **more helpful, safe, and instruction-aligned** using a **two-stage process**:

1. **Supervised Fine-Tuning (SFT)** with LoRA for instruction-following behavior.
2. **Direct Preference Optimization (DPO)** for safety, refusal, and ethical alignment.

> 📘 A detailed research-style report of this project is available in the repo.

---

## 🧠 Project Highlights

- ✅ Instruction tuning with [`databricks-dolly-15k`](https://huggingface.co/datasets/databricks/databricks-dolly-15k)
- ✅ Preference alignment with [`PKU-SafeRLHF`](https://huggingface.co/datasets/PKU-Alignment/PKU-SafeRLHF)
- ✅ Efficient fine-tuning using LoRA (Low-Rank Adaptation)
- ✅ Experiments across **7 SFT trials** and **5 DPO trials**
- ✅ Evaluation via **BLEU scores** and **manual prompt assessments**
- ✅ Interactive Streamlit-based demo UI

---

## 📦 Features

| Phase | Technique | Goal |
|-------|-----------|------|
| **SFT** | LoRA + Instruction Dataset | Teach model to follow instructions accurately |
| **DPO** | Human Preference Dataset | Align model to be safe, helpful, and ethically grounded |
| **Frontend** | Streamlit + LocalTunnel | Demo the model and manually test responses |

---

## 🧰 Tech Stack

- Python 3.10
- Hugging Face Transformers, Datasets, PEFT, TRL
- LoRA (for efficient parameter tuning)
- Streamlit (for app interface)
- Google Colab & Kaggle GPUs (NVIDIA T4)
- Evaluation: BLEU Score + Manual Judgment

---

## 📁 Directory Structure
├── sft_training/ # SFT scripts, logs, and config
├── dpo_training/ # DPO scripts and training runs
├── evaluation/ # Prompts, BLEU scripts, metrics
├── checkpoints/ # LoRA & DPO checkpoint folders
├── app/ # Streamlit frontend
├── report.pdf # Full project report
└── README.md
## 📈 Evaluation Summary

- 🔤 **BLEU Score**: Used to compare base, SFT, and DPO outputs
- 🧪 **Manual Testing**:
  - Helpfulness (Relevance, completeness)
  - Harmlessness (Refusals, safe language)
  - Instruction Alignment (Follows user intent precisely)

> 💡 DPO Trial 3 achieved the best overall balance in performance.

---

## 🚀 Run the App

```bash
cd app
streamlit run app.py

```
---
## Authors
- Rafsha Rahim
- Alina Siddiqui
- Muhammad Ahsan
