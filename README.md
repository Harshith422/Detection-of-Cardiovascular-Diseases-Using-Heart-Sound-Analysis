# Detection of Cardiovascular Diseases Using Heart Sound Analysis  

## 📌 Overview  
This project develops a **machine learning-based system** for detecting **cardiovascular diseases (CVDs)** using **electrocardiogram (ECG) and phonocardiogram (PCG) signals**. Advanced signal processing techniques such as **bandpass filtering, normalization, and Continuous Wavelet Transform (CWT)** are used for feature extraction. The system follows a hierarchical classification approach:  
- **Binary classification**: Detects normal vs. abnormal signals  
- **Multi-class classification**: Identifies specific cardiovascular diseases  

## 🚀 Features  
✅ **Preprocessing** – Bandpass filtering & normalization for noise reduction  
✅ **Feature Extraction** – Continuous Wavelet Transform (CWT) for time-frequency analysis  
✅ **Machine Learning Model** – Support Vector Machines (SVM) for traditional classification  
✅ **Deep Learning Model** – CNN-LSTM hybrid model for improved accuracy  
✅ **Hierarchical Classification** – Binary and multi-class disease classification  

## 🏗️ System Architecture  
The system consists of:  
- **Signal Preprocessing**: Bandpass filtering, normalization, CWT  
- **Feature Engineering**: Extracting meaningful features from ECG & PCG signals  
- **Machine Learning Model**: SVM classifier for binary & multi-class classification  
- **Deep Learning Model**: CNN for spatial patterns + LSTM for temporal dependencies  

## 📜 Project Structure  
```
/cvd-detection
│── data/                          # ECG & PCG dataset
│── preprocessing/                  # Signal processing & feature extraction
│── models/                         # Machine learning & deep learning models
│   ├── svm_classifier.py           # SVM model for classification
│   ├── cnn_lstm_model.py           # CNN-LSTM hybrid model
│   ├── train.py                    # Training script
│   ├── evaluate.py                  # Model evaluation script
│── utils/                          # Helper functions
│── results/                         # Model results, graphs, and logs
│── README.md                        # Project Documentation
│── requirements.txt                  # Dependencies
```

## 🛠️ Installation & Setup  

### 1️⃣ Prerequisites  
- **Python 3.8+**  
- Required libraries (install via `requirements.txt`)  
```bash
pip install -r requirements.txt
```

### 2️⃣ Clone the Repository  
```bash
git clone https://github.com/Harshith422/cvd-detection.git
cd cvd-detection
```

### 3️⃣ Run Preprocessing  
```bash
python preprocessing/data_preprocess.py
```

### 4️⃣ Train Models  
- **SVM Model:**  
```bash
python models/train.py --model svm
```
- **CNN-LSTM Hybrid Model:**  
```bash
python models/train.py --model cnn-lstm
```

### 5️⃣ Evaluate Performance  
```bash
python models/evaluate.py
```

## 🔍 Key Algorithms Used  
### 📊 Continuous Wavelet Transform (CWT)  
- Extracts time-frequency features from ECG & PCG signals  
- Helps detect transient events like murmurs & arrhythmias  

### 🔍 Support Vector Machine (SVM)  
- Used for traditional classification tasks  
- Works with CWT-extracted features  

### 🔮 CNN-LSTM Hybrid Model  
- **CNN** extracts spatial features from wavelet-transformed signals  
- **LSTM** captures temporal dependencies in ECG/PCG signals  

## 📊 Results & Performance  
- **SVM achieved 72.5% accuracy** for binary classification  
- **CNN-LSTM model achieved 79.2% accuracy** for binary classification and 53.4% for multi-class  

## 📄 Future Enhancements  
🔹 **Real-time Monitoring System**  
🔹 **Integration with Wearable Devices**  
🔹 **Explainable AI for Clinical Use**  
