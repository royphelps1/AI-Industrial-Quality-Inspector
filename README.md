# CS614 Final Project
## AI Industrial Quality Inspector

### Overview
This project explores computer vision techniques for automated industrial surface defect detection using transfer learning and explainable AI methods.

The system classifies steel surface defects using a pretrained **ResNet18 convolutional neural network** and provides visual explanations of predictions using **Grad-CAM**.

---

## Objective

The goal of this project is to build a **multi-class image classification system** capable of identifying manufacturing defects from surface images and generating interpretable visual explanations.

Key goals:

- Detect multiple types of industrial surface defects  
- Apply transfer learning to improve performance with limited data  
- Provide explainable predictions using Grad-CAM heatmaps  

---

## Dataset

This project uses the **NEU Surface Defect Dataset**, which contains images of steel surface defects across several classes.

Because the dataset is large, it is **not stored in this repository**.

Download the dataset and place it in the following directory: data/raw/neu_surface_defects/


Dataset source:  
http://faculty.neu.edu.cn/songkechen/zh_CN/zdylm/263270/list/index.htm

---

## Technical Approach

The project uses the following machine learning techniques:

- Transfer Learning with **ResNet18**
- Multi-class image classification
- **PyTorch** deep learning framework
- **Grad-CAM** for explainable AI visualization
- Confusion matrix evaluation and performance metrics

---

## Project Structure

```
CS614-AI-Industrial-Quality-Inspector
│
├── data/
│   └── raw/              (raw dataset – ignored in git)
│
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   └── Final Project.ipynb
│
├── outputs/
│   ├── figures/          (evaluation plots and Grad-CAM examples)
│   └── models/           (trained model checkpoint)
│
├── requirements.txt
└── README.md
```


---

## Setup

Clone the repository:

git clone https://github.com/YOUR_USERNAME/CS614-AI-Industrial-Quality-Inspector.git
cd CS614-AI-Industrial-Quality-Inspector


Install dependencies:
pip install -r requirements.txt


---

## Running the Project

Open and run the final notebook:
notebooks/Final Project.ipynb


The notebook performs the following steps:

1. Load and preprocess the dataset  
2. Train a ResNet18 transfer learning model  
3. Evaluate model performance  
4. Generate confusion matrices and evaluation plots  
5. Produce Grad-CAM visualizations for model interpretability  

---

## Results

The trained model demonstrates effective classification of industrial surface defects and produces interpretable Grad-CAM visualizations highlighting the regions responsible for predictions.

Example outputs include:

- Training accuracy and loss curves
- Confusion matrix
- Example predictions
- Grad-CAM heatmaps

Figures are saved in:
outputs/figures/


---

## Author

Roy Phelps    
Drexel University  
CS614 – Applications of Machine Learning
