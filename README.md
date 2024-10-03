# Project Overview
###### <i>UC Berkeley MIDS `Applied Machine Learning` Group Project</i>

### Objective: 
The goal of this project is to classify breast cancer histopathology slide images into cancerous and non-cancerous categories. The dataset was sourced from the [Kaggle website](https://www.kaggle.com/datasets/paultimothymooney/breast-histopathology-images). We began by training an SVM (Support Vector Machine) as a baseline model and progressively explored more advanced models, including Random Forest, CNN (Convolutional Neural Network), and CNN with transfer learning.

As part of my individual contribution, I focused on building CNNs with five different transfer learning architectures: VGG16, VGG19, ResNet50, ResNet152V2, and DenseNet201. Additionally, I implemented XGBoost and optimized the models using KerasTuner's Random Search to identify the best set of hyperparameters, such as learning rates, the number of layers to unfreeze, dropout rates, and optimizers. My tasks also included extensive exploratory data analysis (EDA) and preprocessing, such as normalizing, resizing, and augmenting the images (e.g., rotation, flipping, shifting, contrast adjustment, etc.). Through Random Search, ResNet50 with the last layer unfrozen was identified as the top-performing model, achieving a test accuracy of 0.76 and a validation accuracy of 0.74, and an Area Under the Curve (AUC) score of 0.92.

For more details on the teamwork, please refer to the link below:
* [Team GitHub](https://github.com/TatiannaD/w207_fall2022_mlproject//)
