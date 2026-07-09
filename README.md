
# AI Skin Lesion Diagnostic Assistant

An end-to-end AI-powered dermatology assistant that analyzes dermoscopic skin lesion images and provides predictions, confidence scores, Grad-CAM visualizations, and clinically relevant lesion information.

Built using React, FastAPI, and deep learning to demonstrate production-ready deployment of computer vision models in healthcare applications.

demp video present in repo !!


---

## Features

- Upload dermoscopic images through drag-and-drop or file picker.
- Real-time skin lesion classification.
- Confidence score visualization.
- Grad-CAM heatmap generation for model interpretability.
- Differential diagnosis suggestions.
- ABCDE melanoma assessment guidance.
- Prediction history tracking.
- Example image gallery for demonstration.
- Modern responsive UI with dark/light theme support.
- Modular architecture designed for future MLOps deployment.

---

## Supported Lesion Classes

The model can classify multiple skin lesion categories including:

- Melanoma (MEL)
- Melanocytic Nevus (NV)
- Basal Cell Carcinoma (BCC)
- Benign Keratosis-like Lesions (BKL)
- Actinic Keratoses (AKIEC)
- Dermatofibroma (DF)
- Vascular Lesions (VASC)

---

## Technology Stack

### Frontend

- React
- Vite
- TailwindCSS
- Context API

### Backend

- FastAPI
- Uvicorn

### Machine Learning

- PyTorch
- Torchvision
- OpenCV
- NumPy
- Pillow

### Explainability

- Grad-CAM

### Deployment

- Docker
- Vercel
- Render

---

## Project Structure

```text
Skin_Lesion/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── ABCDEAssessment.jsx
│   │   │   ├── ConfidenceChart.jsx
│   │   │   ├── DifferentialDiagnosis.jsx
│   │   │   ├── ExampleGallery.jsx
│   │   │   ├── GradCAMViewer.jsx
│   │   │   ├── Header.jsx
│   │   │   ├── HistoryPanel.jsx
│   │   │   ├── ImagePreview.jsx
│   │   │   ├── LesionInfoPanel.jsx
│   │   │   ├── ModelInfo.jsx
│   │   │   ├── PipelineVisualization.jsx
│   │   │   ├── PredictionCard.jsx
│   │   │   ├── UploadArea.jsx
│   │   │   └── UploadCard.jsx
│   │   │
│   │   ├── context/
│   │   ├── data/
│   │   ├── services/
│   │   └── App.jsx
│   │
│   └── package.json
│
├── backend/
│   ├── main.py
│   ├── model.pth
│   ├── requirements.txt
│   └── Dockerfile
│
└── README.md
