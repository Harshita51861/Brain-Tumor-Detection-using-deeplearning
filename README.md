# Brain-Tumor-Detection-using-deeplearning
A PyTorch-based brain tumor MRI classification pipeline using EfficientNet-B0. Includes preprocessing, training, evaluation, prediction logging, and Bias-Aware Grad-CAM explainability. Classifies MRI scans into glioma, meningioma, pituitary tumor, and no tumor.

├── Model Architecture.png      → Architecture diagram
├── deepLearning.ipynb          → Main training & evaluation notebook
├── requirements.txt            → Dependencies
└── README.md                   → Project documentation

Dataset
This project uses the Brain Tumor MRI dataset from Kaggle.
Dataset link:https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset

Installation

Clone the repository:
git clone https://github.com/Harshita51861/Brain-Tumor-Detection-using-deeplearning.git
cd Brain-Tumor-Detection-using-deeplearning

Install dependencies:
pip install -r requirements.txt

How to Run

Download the dataset from Kaggle
Update dataset paths inside the notebook
Run the notebook:
jupyter notebook deepLearning.ipynb

The notebook will automatically:

1.Train EfficientNet-B0
2.Evaluate accuracy
3.Generate confusion matrix
4.Produce Grad-CAM heatmaps
5.Save prediction logs

Output & Evaluation

The notebook generates:

-Accuracy, recall, precision, F1-scores
-Confusion matrix
-Training & validation curves
-Grad-CAM heatmaps for explainability
-Confidence-based predictions
-Prediction logs (prediction_logs.csv)

Explainability (Bias-Aware Grad-CAM):To interpret model predictions, the project uses Bias-Aware Grad-CAM, which averages multiple perturbed heatmaps to highlight reliable tumor-related regions in MRI images.
