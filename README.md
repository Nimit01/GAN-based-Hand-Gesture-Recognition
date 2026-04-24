# Few-Shot ISL Recognition using GAN Augmentation

## Overview
This project focuses on improving Indian Sign Language (ISL) recognition using Computer Vision techniques combined with GAN-based data augmentation.

In few-shot learning scenarios, limited training data leads to poor model performance. This project addresses this issue by generating synthetic data using Generative Adversarial Networks (GANs) and evaluating its impact on classification accuracy.

---

## Objectives
- Develop a gesture recognition system using landmark-based features  
- Improve model performance using GAN-generated synthetic data  
- Compare baseline and augmented models  
- Analyze performance using standard evaluation metrics  

---

## Methodology

### Data Processing
- Extract hand landmarks from images  
- Convert landmarks into structured numerical features  

### Few-Shot Learning
- Train a baseline model using a limited dataset  

### GAN-based Augmentation
- Generate synthetic landmark data  
- Augment the training dataset  

### Model Training
- Train an MLP classifier on:
  - Baseline dataset  
  - Augmented dataset  

### Evaluation
- Test both models on unseen data  
- Compare performance using evaluation metrics  

---

## Model Architecture

### Baseline Model (MLP)
- Input Layer: Landmark Features  
- Hidden Layer 1: 128 units with ReLU and Dropout  
- Hidden Layer 2: 64 units with ReLU and Dropout  
- Output Layer: Number of gesture classes  

---

## Evaluation Metrics
- Accuracy  
- Precision  
- Recall  
- F1-score  

---

## Results
- GAN-augmented model shows improved performance over baseline  
- Better generalization in few-shot learning scenario  
- Reduced misclassification across gesture classes  

---

## Project Structur
data/
│
├── landmarks/
├── augmented/
│
models/
│
├── baseline/
├── fewshot/
│
results/
│
notebooks/
│
├── data_split.ipynb
├── dataset_augmentation.ipynb
├── final_training.ipynb
├── testing_and_evaluation.ipynb
│
README.md


---

## Technologies Used
- Python  
- NumPy  
- Pandas  
- PyTorch  
- Matplotlib  
- Seaborn  
- Generative Adversarial Networks (GANs)  

---

## Key Insights
- Data augmentation improves performance in low-data scenarios  
- GAN-generated samples enhance model generalization  
- Useful for real-world Computer Vision applications  

---

## Future Scope
- Use advanced architectures such as CNNs or Transformers  
- Improve GAN model quality for better synthetic data  
- Extend system for real-time gesture recognition  

---

## References
- https://pytorch.org/  
- https://scikit-learn.org/  
- https://paperswithcode.com/  

---

## Contributors
- Vedant  
- Nimit  
- Vraj
- Varun

---

## Note
The dataset is not included in the repository due to size constraints.
