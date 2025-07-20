# Multimodal_Emotion_Recognition


This project focuses on building a Multimodal Emotion Detection system using **textual data** (as the first modality), with future extensions planned for **audio** and **visual** modalities. The goal is to accurately identify human emotions in conversations by leveraging natural language processing (NLP) and deep learning techniques.

---

## 🧠 Project Objective

To build a deep learning-based **Multimodal Emotion Recognition (MER)** model, starting with training on **textual features** (e.g., BERT embeddings) and expanding to **multimodal fusion** using data from audio and video sources.

---

## 📦 Features

- 🔍 Emotion classification from text using pre-trained transformers (BERT, RoBERTa, etc.)
- 🧪 Fusion-ready architecture to incorporate audio/visual data
- 🗂️ Modular codebase: easy to plug in new modalities
- 📊 Evaluation with standard benchmarks: IEMOCAP, MELD, MOSEI

---

## 🏗️ Project Architecture

```plaintext
           ┌───────────────┐
           │   Raw Text    │
           └─────┬─────────┘
                 ▼
          ┌────────────┐
          │ Tokenizer  │
          └────┬───────┘
               ▼
      ┌──────────────────┐
      │ BERT Embeddings  │
      └────────┬─────────┘
               ▼
       ┌──────────────┐
       │ Classifier   │  ← (LSTM / FFN / Softmax)
       └──────────────┘
               ▼
       ┌──────────────┐
       │ Emotion Tag  │ → [Happy, Sad, Angry, Neutral, etc.]
       └──────────────┘



## 📚 Datasets Used
	•	IEMOCAP
	•	MELD
	•	CMU-MOSEI


🔧 Setup Instructions
# Clone the repo
git clone https://github.com/your-username/multimodal-emotion-detection.git
cd multimodal-emotion-detection

# Create virtual environment
python -m venv venv
source venv/bin/activate  # or .\venv\Scripts\activate on Windows

# Install dependencies
pip install -r requirements.txt


## 🚀 Training (Text Modality)
python train_text_model.py --model bert --dataset iemocap
Options:
	•	--model: [bert, roberta, distilbert]
	•	--dataset: [iemocap, meld, mosei]

## 📈 Evaluation

python evaluate.py --checkpoint saved_models/text_bert.pth

Metrics:
	•	Accuracy
	•	Precision, Recall, F1
	•	Confusion Matrix

## 🛠️ Future Work
	•	Integrate Audio modality (OpenSMILE + CNN/RNN)
	•	Integrate Video modality (3D CNNs or facial expression detectors)
	•	Fusion via Attention, MLP, or Gated Networks
	•	Real-time prediction API

## 📄 References
	•	MEmoBERT: Prompt-based Multimodal Emotion Recognition
	•	Survey: Multimodal Emotion Recognition in Conversations (2025)
	•	CMU-MOSEI Dataset

⸻

## 🤝 Contributing

Feel free to open issues or submit pull requests to improve the project.

## 📃 License

MIT License © 2025 Pritam Pani
