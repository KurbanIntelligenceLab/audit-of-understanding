# 🧠 Audit-of-Understanding (AoU): Think Before You Guess

**Audit-of-Understanding (AoU)** is a prompting framework for improving faithfulness in LLM reasoning. It encourages models to **explicitly state and verify their assumptions** before producing an answer — reducing hallucinations, improving transparency, and yielding higher accuracy on symbolic and mathematical tasks.

Rather than asking a model to "just solve" a problem, AoU breaks the process into three structured stages:

1. **Assume** – List minimal assumptions, facts, or intermediate steps  
2. **Audit** – Evaluate each assumption as **SUPPORTED** or **MISSING**  
3. **Answer** – Solve the problem using only supported information

---

## 🚀 Features

- 🧠 **Bayesian-inspired reasoning** via assumption auditing  
- 🔍 **Hallucination control** by constraining to verifiable inputs  
- 🧪 **Plug-and-play**: No fine-tuning or tools required
- 📊 Tested on GSM8k, SVAMP, MultiArith with strong performance gains

---

## 📁 Repo Structure

- **pipeline.ipynb** # Main 3-stage pipeline (assume → audit → solve)
- **/data** # csv files for some datasets (others directly from huggingface)
- **baselines.ipynb** # Baselines such as CoT, Self Consistency and CoT-decoding used for comparison
- **README.md** # You're here!

---

## 🚀 Getting Started

Follow these steps to use the dataset and run benchmarks.

### 1. Clone the Repository

```bash
git clone https://github.com/KurbanIntelligenceLab/audit-of-understanding.git
cd audit-of-understanding
```

### 2. Downloading dependencies

Download all required dependencies 


### 3. Creating output directory  the Dataset

```bash
mkdir output
```

### 4. Login to huggingface through terminal (ensure that you have access to all required models to run experiment)

```bash
!huggingface-cli login
```

### 5. Run pipeline.ipynb


