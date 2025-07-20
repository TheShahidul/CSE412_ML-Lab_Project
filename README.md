
# 🩺 Medical Assistant System using Machine Learning

A terminal-based intelligent healthcare assistant designed to predict diseases based on user-provided symptoms or image-based input using OCR, with detailed guidance on medications, precautions, diets, and workouts.

> 🎓 Developed as part of the Machine Learning Lab (CSE 412) at Green University of Bangladesh, Fall 2024.

---

## 📌 Project Overview

The **Medical Assistant System** utilizes a supervised machine learning model (Support Vector Classifier) to predict diseases based on symptoms provided either manually or through OCR-extracted text from medical images.

The goal is to provide **accessible and intelligent medical assistance**—particularly for regions with limited access to professional healthcare—by offering early and informed disease prediction and guidance.

---

## 🧠 Features

- 🔍 **Disease Prediction** from symptom selection or OCR-based input  
- 🖼️ **OCR Support** for extracting symptoms from images (e.g., prescriptions, notes)  
- 🧾 **Detailed Medical Insights**: Description, medications, precautions, diets, and workout suggestions  
- 🖥️ **Graphical User Interface (GUI)** built using Tkinter for ease of use  
- 💾 Save results locally and re-initiate prediction seamlessly  
- ⚙️ Simple terminal and GUI-based operation  

---

## 🖼️ User Interface

The interface includes:

- Multi-symptom selection with prediction output  
- OCR image upload option  
- File save functionality  
- Reset and re-prediction support  

> **Built using Python's Tkinter for intuitive interaction.**

---

## 🏗️ System Architecture

```
Symptom Input (Manual / OCR Image)
              ↓
Symptom Processing (Normalization, Encoding)
              ↓
ML Model (SVC) → Prediction
              ↓
Output: Disease Name + Medications + Diet + Workout + Precautions
```

---

## 🛠️ Tech Stack

| Component           | Tools/Libraries          |
|---------------------|--------------------------|
| Language            | Python 3.x               |
| GUI                 | Tkinter                  |
| Machine Learning    | scikit-learn (SVC model) |
| OCR                 | Tesseract OCR + Pillow   |
| Data Handling       | pandas, numpy            |
| Model Persistence   | pickle                   |

---

## 📦 Dataset

Includes CSV files for:

- Symptoms (`symptoms_df.csv`)  
- Descriptions (`description.csv`)  
- Medications (`medications.csv`)  
- Diets (`diets.csv`)  
- Precautions (`precautions_df.csv`)  
- Workouts (`workout_df.csv`)  

The dataset maps symptoms to diseases and associates each disease with a range of supporting healthcare suggestions.

---

## 📈 Performance

- ✅ High accuracy for common disease predictions  
- 📷 OCR performs well with clear images; accuracy may drop with poor quality  
- ⚠️ Not intended to replace professional medical advice  

---

## 🚀 How to Run

### 🔧 Prerequisites

- Python 3.x  
- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) installed and added to system path  

### 💻 Installation

```bash
# Clone the repository
git clone https://github.com/TheShahidul/CSE412_ML-Lab_Project.git
cd CSE412_ML-Lab_Project

# Create virtual environment (optional but recommended)
python -m venv env
source env/bin/activate  # For Windows: env\Scripts\activate

# Install dependencies
pip install numpy pandas scikit-learn pytesseract pillow
```

### ▶️ Run the App

```bash
python main.py
```

This will launch the Tkinter GUI.

---

## 🧪 Testing & Evaluation

- Developed and tested in **Visual Studio Code**  
- Simulation includes:
  - Symptoms-only input  
  - OCR image input  
  - UI interaction and save functionality  

---

## ❗ Limitations

- Dataset coverage is limited to common diseases  
- OCR may misread handwritten or poorly scanned images  
- Black-box nature of the ML model reduces interpretability  
- Not designed for emergency diagnosis or real-time processing  

---

## 🌱 Future Improvements

- 📚 Expand dataset to cover more diseases  
- 🤖 Integrate deep learning for improved OCR  
- 💬 Add support for natural language queries  
- 📲 Develop a mobile app version  
- 🩺 Collaborate with healthcare experts for validation  
- 🧠 Incorporate Explainable AI for better model transparency  

---

## 👨‍💻 Authors

- Md. Shahidul Islam Prodhan – [GitHub](https://github.com/TheShahidul)  
- Nazmul Hasan  

---

## 📄 License

This project is part of an academic course and is intended for educational and demonstrative purposes only. Not to be used for actual medical diagnosis.

---

## 📚 References

Includes works from NEJM, Springer, Journal of Healthcare Engineering, and others.  
For the complete reference list, refer to the [📘 Project Report](./CSE412_ML-Project-Report.pdf).

---

## 🧾 Acknowledgements

- **Instructor**: Md. Atikuzzaman, Green University of Bangladesh  
- Open-source libraries and medical datasets used during development  

---
