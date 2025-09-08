# Alzheimer's Disease Classification using Deep Learning

This project investigates the predictive capabilities of **Convolutional Neural Networks (CNNs)** and **transfer learning models** (Inception V3, ResNet-18, ResNet-50) for the progression and early detection of **Alzheimer’s Disease (AD)**.  

Alzheimer’s disease prediction plays a critical role in **early intervention and patient care**, and this work contributes to developing reliable, efficient deep learning approaches for diagnosis.

---

## Dataset

- **Source**: [Alzheimer’s Disease Neuroimaging Initiative (ADNI)](http://adni.loni.usc.edu/)  
- **Data types**: multimodal neuroimaging, clinical, genetic, and demographic data  
- **Preprocessing**:  
  - Image normalization  
  - Feature extraction and engineering  
  - Preparation for deep learning model training  

---

## Models Implemented

The repository contains multiple Jupyter Notebooks exploring different modeling approaches:

- **CNN.ipynb** → Baseline Convolutional Neural Network implementation  
- **CNN_on_mri.ipynb** → CNN model trained specifically on MRI data  
- **CNN_hybrid.ipynb** → Hybrid CNN with additional feature inputs  
- **SVM_onMRI.ipynb** → Support Vector Machine (SVM) classifier for MRI data  
- **Oasis_algos.ipynb / MLalgos_oasis.ipynb** → Traditional ML algorithms on OASIS dataset  
- **ADNI_CNN(leakyrelu).ipynb** → CNN on ADNI dataset with LeakyReLU activation  

---

## Results

Performance was evaluated using **accuracy, precision, recall, and F1 score**, with **k-fold cross-validation** for robustness.  

| Model        | Accuracy |
|--------------|----------|
| CNN          | 93.75%   |
| Inception V3 | 94.06%      |
| ResNet-50    | 88.33%     |
| ResNet-18    | 50.83%     |

**Key finding**: CNN and Inception V3 demonstrated the strongest performance, showing their effectiveness in modeling AD progression.

---

##  Installation & Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/bhumi1306/Alzheimers_Disease_Classification.git
   cd Alzheimers_Disease_Classification
2. Create and activate a Python environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate   # (Linux/Mac)
   venv\Scripts\activate      # (Windows)

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
4. Open Jupyter Notebook to explore models:
   jupyter notebook
   
## Usage

Run any notebook of interest (e.g., CNN.ipynb, InceptionV3.ipynb).

Ensure the dataset is properly downloaded and preprocessed (ADNI dataset requires request & approval).

Modify hyperparameters, model layers, and preprocessing steps as needed.
