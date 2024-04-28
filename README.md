# Transfer-Learning-for-NLP-with-TensorFlow-Hub

------------------------------

## Project Overview

**In this project**, the aim is to address the challenge of improving the quality of online discussions by focusing on the detection of toxic content. As a case study, the analysis of questions asked on Quora has been chosen -a platform known for its diverse user-generated content. The goal is to develop a predictive model that can accurately label questions as either sincere or insincere.

### Dataset Information

The dataset used in this project is the Quora Insincere Questions Classification dataset, which can be accessed on [Kaggle](https://www.kaggle.com/c/quora-insincere-questions-classification/data).I use a fraction of the Quora Insincere Questions dataset (`train.csv`) due to the extensive pre-training of our text classification models. However, you can choose to utilize the entire dataset if needed.

Insincere questions are those that exhibit characteristics such as a non-neutral tone, disparaging language, the inclusion of inflammatory content based on false information, or the presence of sexually explicit content intended to shock or provoke. By identifying and flagging these insincere questions, we can contribute to creating a healthier and more respectful online environment.

### Inspiration

**This project draws inspiration** from the Coursera project [Transfer Learning for NLP with TensorFlow Hub](https://www.coursera.org/projects/transfer-learning-nlp-tensorflow-hub/), with modifications to enhance visualization and conceptual understanding.


## Methodology

- I utilize pre-trained models from TensorFlow Hub with `tf.keras` for text classification.
- Transfer learning enables fine-tuning models on text data, saving training resources and achieving good model generalization.
- Model performance metrics are visualized using [TensorBoard](https://www.tensorflow.org/tensorboard).

### Why Transfer Learning in NLP?

Transfer learning leverages shared knowledge about language across NLP tasks, improving model performance and efficiency. This is because many NLP tasks share common linguistic representations and structural similarities in language. When performing these tasks, they can inform and benefit from each other, making transfer learning a powerful approach in NLP.

## Text Data and Representations

Our dataset comprises questions paired with corresponding labels. To train the statistical classification model effectively, we use question vectors as distributed representations of the questions. These question vectors, along with their corresponding labels, are employed during training to build and fine-tune the model.

## Table of Contents

1. **Check GPU Availability**
2. **Importing Necessary Libraries**
3. **Download and Import Dataset**
4. **Text Embedding Explanations and TensorFlow Hub**
5. **Define Function to Build and Compile Models**
6. **Train Various Text Classification Models (without fine-tuning)**
7. **Train Various Text Classification Models (with fine-tuning)**
8. **Compare Accuracy and Loss Curves**
9. **Visualize Metrics with TensorBoard**


## Recap

**This project demonstrates:**
- Usage of pre-trained NLP text embedding models from TensorFlow Hub.
- Transfer learning and fine-tuning on real-world text data.
- Visualization of model performance metrics using Matplotlib, TensorFlow documentation package, and TensorBoard.

## References

1. **Quora Insincere Questions Classification Dataset**:
   - **Authors**: Alex Ellis, inversion, Julia Elliott, Paula Griffin, William Chen
   - **Title**: Quora Insincere Questions Classification
   - **Publisher**: Kaggle
   - **Year**: 2018
   - **URL**: [Quora Insincere Questions Classification](https://www.kaggle.com/c/quora-insincere-questions-classification/data)

2. **Coursera Project**:
   - **Title**: Transfer Learning for NLP with TensorFlow Hub
   - **Publisher**: Coursera
   - **URL**: [Transfer Learning for NLP with TensorFlow Hub](https://www.coursera.org/projects/transfer-learning-nlp-tensorflow-hub/)
