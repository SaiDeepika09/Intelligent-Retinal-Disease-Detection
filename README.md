# Intelligent Retinal Disease Detection Using OCT Images

## 1. Project Overview

This project focuses on detecting retinal diseases using Optical Coherence Tomography (OCT) images and Deep Learning techniques.

A Custom Convolutional Neural Network (CNN) was developed to classify OCT images into four categories:

- CNV (Choroidal Neovascularization)
- DME (Diabetic Macular Edema)
- DRUSEN
- NORMAL

The project also includes a Streamlit web application that allows users to upload OCT images and view the predicted disease category and confidence score.

## 2. Technologies Used

- Python
- PyTorch
- Torchvision
- Streamlit
- NumPy
- Pillow
- Matplotlib
- Scikit-learn

## 3. Dataset

Dataset: Kermany2017-OCT

Source: https://huggingface.co/datasets/zacharielegault/Kermany2017-OCT

The dataset contains four image categories: CNV, DME, DRUSEN, and NORMAL.

## 4. Models Developed

The following models were explored:

- Custom CNN
- ResNet18
- VGG16
- Optimized CNN
- Tuned CNN

Custom CNN and ResNet18 were selected for final test evaluation.

## 5. Model Evaluation

The Custom CNN achieved the following results on the test dataset:

| Metric | Score |
|---|---:|
| Accuracy | 87.90% |
| Weighted Precision | 90.90% |
| Weighted Recall | 87.90% |
| Weighted F1-score | 87.44% |

ResNet18 achieved a test accuracy of 73.50%.

Based on the comparison, Custom CNN was selected as the final model.

## 6. Streamlit Application

The application provides:

- OCT image upload
- Uploaded image display
- Retinal disease prediction
- Prediction confidence score
- Medical disclaimer

## 7. Model Explainability

Grad-CAM was implemented to visualize image regions influencing the Custom CNN prediction.

## 8. Project Structure

```text
Retinal Disease Detection/
│
├── data/
├── models/
│   └── custom_cnn_model.pth
├── results/
├── images/
├── app.py
├── requirements.txt
├── README.md
└── oct_env/
```

## 9. How to Run the Application

1. Clone or download the project.
2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

3. Run the Streamlit application:

```bash
streamlit run app.py
```

## 10. Disclaimer

This application is developed for educational and research purposes only. Its predictions should not be considered a medical diagnosis or used as a substitute for professional medical advice.