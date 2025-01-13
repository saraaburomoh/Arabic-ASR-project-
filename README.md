# **Fine-tuning ArTST for Arabic ASR**

This project focuses on fine-tuning the ArTST (Arabic Text and Speech Transformer) model for Automatic Speech Recognition (ASR) tasks using the **Classical Arabic TTS Corpus (ClArTTS)** dataset. The model, based on the SpeechT5 architecture, is pre-trained on Modern Standard Arabic (MSA) speech and text data and fine-tuned for specific ASR tasks.

---

## **Overview**

- **Dataset**: [Classical Arabic TTS Corpus (ClArTTS)](https://huggingface.co/datasets/MBZUAI/ClArTTS)
- **Model Architecture**: SpeechT5-based ArTST for ASR
- **Implementation**: Developed using Google Colab with support for GPU acceleration.

---

## **Dataset Summary**

The **Classical Arabic TTS Corpus (ClArTTS)** is designed to support the development of end-to-end Text-to-Speech (TTS) systems for Arabic. It contains:

- Approximately **12 hours of speech** data from a single male speaker.
- Audio sampled at **40,100 kHz**, transcribed and annotated manually.

### **Dataset Structure**
Each data point includes:
- **File**: The name of the audio file.
- **Text**: The transcription of the audio.
- **Audio**: The audio file as an array.
- **Additional Information**: Sampling rate and duration of the audio.

---

## **Steps to Run the Code**

### **1. Set Up the Environment**
- Install the required libraries:
  ```bash
  pip install -q transformers datasets librosa evaluate jiwer accelerate transformers[torch] pyarabic sentencepiece
