# Assignment 3 — Reinforcement Learning from Human Feedback (RLHF) with GPT

In this assignment, we explore **Reinforcement Learning from Human Feedback (RLHF)** to fine-tune a GPT-style language model using the `trl` library. This technique improves model behavior using preference-based rewards — a method used in models like ChatGPT.

---

## 🧠 Objective

To simulate the RLHF process on a language generation task by:
- Fine-tuning a pre-trained model (e.g., GPT-2)
- Using reward modeling and PPO training
- Observing performance differences before and after RLHF

---

## ⚙️ Tools & Libraries

| Library | Purpose |
|--------|---------|
| 🤗 `transformers` | Base language model (e.g., GPT-2) |
| 🎮 `trl` | Training loop for RLHF (PPOTrainer) |
| 📈 `tqdm` | Training progress bar |
| 🧪 `torch` | Backend tensor operations |

---

## 🔁 Process Overview

1. **Load base GPT model** using Hugging Face Transformers
2. **Create prompts** and initial generation samples
3. **Define a reward function** (or mock it)
4. **Train using PPO (Proximal Policy Optimization)** from the `trl` library
5. **Evaluate** how output changes after training

---

## 📂 Project Structure

- `HW_RLHF_gpt.ipynb` — Notebook with full RLHF pipeline
- `README.md` — Project overview and documentation

---

## 📊 Output Analysis

- Compare generations **before and after RLHF**
- Use qualitative or BLEU-style scoring to measure improvements

---

## 💡 Future Improvements

- Use real human feedback or synthetic reward models
- Test on longer text or dialogue generation tasks
- Apply RLHF on larger models (e.g., `gpt2-medium`, `opt`, `llama2`)

---

## 📌 Status

✅ RLHF process implemented via PPO  
✅ Model trained with custom reward signals  
✅ Improved output generation quality

---

## 📜 License

This project is part of the Deep Learning Spring 2025 coursework and is intended for academic use.
