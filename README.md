# Vision-Language Text Extraction using LLama 3.2 and LoRA Fine-Tuning

This project focuses on extracting text from images using Vision Language Models (VLMs), specifically the LLama 3.2 11B Vision model. It evaluates the quality of extracted text using Word Error Rate (WER) and Character Error Rate (CER), and fine-tunes the model using parameter-efficient techniques (LoRA) to reduce these error metrics.

---

## 📂 Dataset
- The dataset used includes image-text pairs, aimed at extracting embedded text in visuals.
- Human-annotated and OCR-generated text is used to construct ground truth labels.
- Train-test split is created for both baseline inference and fine-tuning phases.

---

## 🚀 Objectives

1. **Perform baseline inference** using LLama 3.2 Vision Model.
2. **Evaluate performance** using WER and CER.
3. **Fine-tune** the model using LoRA to improve extraction quality.
4. **Compare** baseline vs fine-tuned performance.
5. **Organize extracted text** to improve readability.

---

## 🧠 Key Techniques

- **LLama 3.2 11B Vision Model** for baseline inference.
- **LoRA (Low-Rank Adaptation)** for efficient fine-tuning.
- **Error Metrics:**
  - `Word Error Rate (WER)`
  - `Character Error Rate (CER)`

---

## 📈 Evaluation Metrics

| Phase           | WER ↓ | CER ↓ |
|----------------|-------|-------|
| Baseline       | High  | High  |
| After Fine-Tune| Lower | Lower |

*Note: ↓ indicates that lower values are better.*

---

## 📊 Results
Fine-tuning the LLama 3.2 model using LoRA led to a reduction in both WER and CER, improving the overall text extraction performance significantly.

---

## 🛠️ Tech Stack

- Python
- Hugging Face Transformers
- LLama 3.2 Vision Model
- LoRA (via PEFT library)
- NumPy, Pandas
- Matplotlib / Seaborn (optional, for visualization)
- jiwer (for WER/CER calculation)


---

## 📁 Files

- `VLM_Final.ipynb`: Complete code notebook with baseline, fine-tuning, evaluation, and comparison.


---

## 📌 How to Run

1. Clone the repo and install requirements.
2. Place dataset as per paths defined in notebook.
3. Run all cells in order.
4. Review WER and CER values in outputs.

---

## 📚 Reference

- LLama 3.2 Vision Model from Meta
- HuggingFace Transformers & PEFT
- jiwer (WER/CER): https://pypi.org/project/jiwer/

---
