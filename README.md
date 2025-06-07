
---

# **LipSync: AI-Powered Visual Speech Recognition for the Hearing Impaired** 👁️‍🗨️  

LipSync is a cutting-edge deep learning-based **Visual Speech Recognition (VSR)** system designed to convert silent lip movement videos into transcribed text. Built with **Conv3D + BiLSTM** architecture and trained on the **GRID corpus dataset**, LipSync enables seamless communication support for individuals with hearing impairments—functioning purely on visual input, unaffected by noise or sound-sensitive environments.

## 🚀 **Key Features**  

✅ **Deep Learning Architecture:** 3D CNNs + BiLSTMs for accurate lip-based speech recognition  
✅ **End-to-End Character-Level Transcription:** Uses **CTC Loss** for alignment-free decoding  
✅ **Trained on GRID Corpus:** Structured English sentence prediction from visual speech  
✅ **Robust Evaluation Metrics:** WER, SER, F1-score, Confusion Matrix analysis  
✅ **High Accuracy:** Achieved **90.36% Weighted F1-score**  
✅ **Lightweight UI with Streamlit:** Real-time processing & demos  
✅ **Optimized for GPU Training:** Supports **RTX 4060** and higher  

---

## 🏗 **System Architecture**  

```plaintext
[Video Input] → [Frame Extraction] → [Mouth ROI Cropping]  
→ [Conv3D Layers] → [MaxPooling3D]  
→ [BiLSTM Layers] → [Dense + Softmax]  
→ [CTC Loss Training] → [Predicted Text Output]
```

---

## 📂 **Dataset: GRID Corpus**  
- **~34,000** structured video samples  
- Includes **aligned video-transcript pairs**  
- Used for **model training & evaluation**  

---

## 🔧 **Tech Stack**  

| **Domain** | **Tools / Frameworks** |
|------------|-----------------------|
| Deep Learning | TensorFlow 2.10, Keras |
| UI | Streamlit |
| Preprocessing | OpenCV, NumPy |
| Language | Python 3.8+ |
| Evaluation | WER, SER, F1 Score, Confusion Matrix |
| Deployment | Local GUI with `.h5` + `.pkl` models |

---

## 🚀 **Getting Started**  

### ✅ **Prerequisites**  
- **Python 3.8+**  
- **NVIDIA GPU (Recommended: 8GB+ VRAM)**  

### 🏃 **Installation & Execution**  

Clone the repository and install dependencies:  
```sh
pip install -r requirements.txt
```

Run the application via Streamlit:  
```sh
streamlit run streamlit_app.py
```

Upload a `.mpg` video from **GRID corpus**, click "Analyze Video," and view the transcribed output.

---

## 📈 **Model Performance**  

| **Metric** | **Value** |
|------------|---------|
| Accuracy | **90.38%** |
| F1 Score (Weighted) | **0.9036** |
| Word Error Rate (WER) | **~9.6%** |
| Sentence Error Rate (SER) | **~11%** |

Includes **confusion matrix**, accuracy plots, and training logs.

---

## 🔮 **Future Scope**  
🔹 **Real-time webcam lip reading**  
🔹 **Multilingual visual speech recognition**  
🔹 **Advanced CTC decoding (e.g., Beam Search)**  
🔹 **Audio-visual fusion models**  
🔹 **Mobile & embedded deployment (TensorFlow Lite / ONNX)**  
🔹 **Emotion-aware lip reading**  
🔹 **Explainable AI (e.g., lip attention heatmaps)**  
🔹 **Cloud-hosted interface enhancements**  

---

## 📚 **References**  
- **GRID Corpus**  
- **TensorFlow 2.10**  
- **LipNet (Assael et al.)**  
- **LRS3 / LRW Datasets**  
- **BiLSTM, Conv3D, CTC Loss**  
- **Streamlit, OpenCV**  

---

😊
