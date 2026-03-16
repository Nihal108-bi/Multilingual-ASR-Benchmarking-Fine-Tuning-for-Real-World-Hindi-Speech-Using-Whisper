# 🎙️ Multilingual ASR Benchmarking & Fine-Tuning for Real-World Hindi Speech

An end-to-end research-oriented project evaluating and improving Automatic Speech Recognition (ASR) performance on real-world Hindi audio using OpenAI Whisper.

---

## 🚀 Overview

Voice interfaces are becoming the primary interaction layer between humans and machines. However, speech recognition systems often degrade significantly in real-world conditions such as noise, accents, and code-switching.

This project builds a complete pipeline to:

* Evaluate baseline ASR performance on Hindi speech
* Test robustness under noisy conditions
* Fine-tune a state-of-the-art model on domain data
* Analyze failure modes
* Demonstrate measurable improvements

---

## 🎯 Objectives

* Benchmark Whisper on multilingual Hindi speech
* Simulate real-world environments with noise augmentation
* Reduce Word Error Rate (WER) through fine-tuning
* Perform detailed error analysis
* Build a reproducible ASR evaluation framework

---

## 🧠 Why This Project Matters

Real-world speech AI systems must handle:

* Diverse accents
* Code-switched speech (Hindi + English)
* Background noise
* Informal speaking styles

This work mirrors how production ASR systems are evaluated and improved in industry.

---

## 🗂️ Dataset

**Mozilla Common Voice — Hindi**

* Public multilingual speech dataset
* Thousands of speakers
* Real recorded audio samples
* Human-verified transcripts

Dataset characteristics analyzed:

* Audio duration distribution
* Transcript length distribution
* Real sample inspection

---

## ⚙️ Methodology

### 1️⃣ Baseline Evaluation

Evaluate pre-trained Whisper on clean Hindi speech.

### 2️⃣ Noise Robustness Testing

Add synthetic noise to simulate real-world conditions and measure degradation.

### 3️⃣ Fine-Tuning

Adapt the model to domain data to improve recognition accuracy.

### 4️⃣ Comparative Benchmarking

Compare performance across:

* Clean audio
* Noisy audio
* Fine-tuned model

### 5️⃣ Error Analysis

Inspect failure cases to identify systematic weaknesses.

---

## 📊 Evaluation Metrics

* **Word Error Rate (WER)** — primary ASR metric
* **Character Error Rate (CER)** — sensitive to spelling errors

Lower values indicate better performance.

---

## 📈 Results

| Condition  | WER ↓        | CER ↓        |
| ---------- | ------------ | ------------ |
| Baseline   | 0.933917     |0.591408      |
| Noisy      |1.471338      |1.292568      |
| Fine-Tuned | **0.405255** | **0.171684** |


---

## 🔍 Key Findings

* Performance drops significantly under noisy conditions
* Fine-tuning improves recognition accuracy on domain speech
* Errors frequently occur on long sentences and rare words
* Real-world deployment requires noise-robust training data

---

## 🎧 Real-World Demo

The notebook supports transcription of custom audio samples, enabling practical testing beyond benchmark datasets.

---

## 🏗️ Tech Stack

* Python
* PyTorch
* Hugging Face Transformers
* Whisper ASR
* Datasets Library
* JiWER (evaluation metrics)

---

## 📂 Project Structure

```
notebook.ipynb          # End-to-end pipeline
benchmark_results.csv   # Performance comparison
prediction_analysis.csv # Error analysis outputs
```

---

## 🧪 Reproducibility

The project is fully reproducible using Google Colab with GPU support.

---

## 🚀 Potential Extensions

* Code-switching evaluation (Hinglish)
* Accent robustness testing
* Real-world noise datasets
* Speech-to-speech systems
* Deployment as a voice assistant backend

---

## 👨‍💻 Author

Nihal Jaiswal
Aspiring AI/ML Engineer specializing in Machine Learning, NLP, and Speech AI.

---

## ⭐ If you find this project useful, consider giving it a star!
