# BTTAI-AJL-Team-5

## **🎯 Project Highlights**

* Built a CNN model using ReLU activation to support inclusive healthcare diagnostics.
* Focused on reducing bias in dermatology by training on diverse skin tones.
* Achieved 31% accuracy.
* Used data encoding and image generators to efficiently process images within computing limits.

🔗 [Equitable AI for Dermatology | Kaggle Competition Page](https://www.kaggle.com/competitions/bttai-ajl-2025/overview)

---
## **👩🏽‍💻 Setup & Execution**

### How to clone the repository
Follow [this instruction](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository). 

### How to access the dataset(s)
You can download the training and testing data from the [competition site](https://www.kaggle.com/competitions/bttai-ajl-2025/data).
  
### How to run the notebook or scripts
Our notebook was created on Kaggle, so the easiest way to run it is to use Kaggle’s platform itself. Kaggle will automatically handle the environment, dependencies, and all the required settings for you. 

If you want to run the notebook locally, open the .ipynb file using Jupyter Notebook, Python, or any other IDE you prefer. If any dependencies are missing, install them using pip: ```pip install <package-name>```

---
## **🏗️ Project Overview**

### About the Kaggle Competition
This project is part of a Kaggle competition presented by Break Through Tech AI in collaboration with the [Algorithmic Justice League (AJL)](https://www.ajl.org/about). Participants include AI Fellows from the Virtual, Boston (MIT), and Los Angeles (UCLA) programs.

### Objective of the Challenge
The goal of this challenge is to develop a machine learning model that accurately classifies skin conditions across diverse skin tones. This is a critical issue in dermatology, where existing models often fail to diagnose conditions accurately in patients with darker skin tones due to biased and unrepresentative training data.

### Real-World Significance
AI has rapidly changed industries, including healthcare, by automating complex tasks like diagnosing medical conditions. However, many AI models are built using biased and unbalanced datasets, making them less effective for diverse populations.

In dermatology, AI models often struggle to identify skin conditions on a wide range of skin tones. This leads to misdiagnosis and delayed treatment, especially for low-income communities of color. These biases reinforce existing healthcare disparities and put vulnerable groups at greater risk.

As data and machine learning engineers, we have a responsibility to challenge these biases and develop fair, inclusive AI models. Through this project, we aim to reduce bias in dermatology AI models by training on more diverse and representative data. Our goal is to build a highly accurate model that improves healthcare for vulnerable communities, so that all patients receive accurate and reliable diagnoses, regardless of their skin tone.


---
## **📊 Data Exploration**

For our CNN model, we used data provided by AJL which includes about 4,500 images representing roughly 21 skin conditions with a range of skin tones. 

For pre-processing the dataset, we augmented the images to introduce randomness and variety by applying random transformations (like rotation, flipping, zooming, or shifting) to the original images.

We assume that all the data files (image file paths) are working.

---
## **🧠 Model Development**

**Model Used:**
* A sequential Convolutional Neural Network (CNN) was implemented using TensorFlow Keras to classify skin conditions from images.
* CNNs are well-suited for this task because they can learn hierarchical features, making them effective for analyzing skin images, such as texture, color, and skin condition.

**Feature Selection & Hyperparameter Tuning:**
* **Feature Selection:**
  * No manual feature selection was performed.
  * Data augmentation techniques (rotation, flipping, scaling) were used to enhance the training dataset and improve generalization.

* **Model Adjustments:**
  * Batch Normalization: Applied after each convolutional layer to stabilize training and improve performance.
  * Max Pooling: Used after each convolutional block to reduce dimensionality while preserving important features.
  * Dropout: Added in fully connected layers with a 0.5 probability to prevent overfitting.

* **Hyperparameter Tuning:**
  * Optimizer: Adam with a learning rate of 0.00005.
  * Loss function: Sparse categorical cross-entropy.
  * Early Stopping: Monitored validation loss with a patience of 7 epochs to prevent overfitting and restore the best weights.

**Training Setup:**
* **Data Split:**
  * 80% for training and 20% for validation.
    
* **Image Preprocessing:**
  * Images were preprocessed using data generators, resized to 128x128 pixels, and batch normalized to improve training efficiency.
    
* **Training Details:**
  * Trained for 30 epochs with accuracy as the evaluation metric.
  * Early stopping ensured the model did not overfit during training.
  * The trained model was saved as `dermatology_cnn.h5` for further use and evaluation.

---
## **📈 Results & Key Findings**

Our model achieved an **accuracy of 31%** on the validation set and ranked **37th on the Kaggle leaderboard**. We used the F1-score as the primary metric to balance precision and recall, as minimizing false negatives was crucial for this task. Overall, the model performed decently and learned useful patterns, but it wasn’t perfect. The model did better on lighter skin tones but struggled with darker skin tones. This revealed fairness issues in the model. A model that performs well overall may still fail for certain groups. To address this, we would incorporate more diverse data, especially from darker skin tones. We would also test the model for equity across all groups to prevent real-world discrimination.

---
## **🖼️ Impact Narrative**
**AJL challenge:**

As Dr. Randi mentioned in her challenge overview, “Through poetry, art, and storytelling, you can reach others who might not know enough to understand what’s happening with the machine learning model or data visualizations, but might still be heavily impacted by this kind of work.”

As you answer the questions below, consider using not only text, but also illustrations, annotated visualizations, poetry, or other creative techniques to make your work accessible to a wider audience. Check out [this guide](https://drive.google.com/file/d/1kYKaVNR\_l7Abx2kebs3AdDi6TlPviC3q/view) from the Algorithmic Justice League for inspiration!

1. What steps did you take to address [model fairness](https://haas.berkeley.edu/wp-content/uploads/What-is-fairness_-EGAL2.pdf)? (e.g., leveraging data augmentation techniques to account for training dataset imbalances; using a validation set to assess model performance across different skin tones)

To check how fair our model was, we tested its performance on different skin tones. We found that it performed better on lighter skin tones and struggled with darker skin tones, showing that it wasn’t treating all skin tones equally. To address this, we used data augmentation techniques to add more variety to the training images, especially for darker skin tones. We also thought about adding more images of people with darker skin to make the dataset more balanced. Unfortunately, we didn’t have time to implement all of these changes, but it really opened our eyes to how important fairness is in model development.

2. What broader impact could your work have?

The idea behind our model has a lot of potential to improve healthcare equity, especially in image analysis for diverse groups. However, to make sure it works fairly for everyone, further improvements are needed. This project highlights the need to build models that provide equitable outcomes, benefiting all groups, not just specific ones.

---

## **🚀 Next Steps & Future Improvements**

* **Limitations of the Model:**
Our model didn’t always produce accurate results, especially when it came to darker skin tones. It struggled with these and was generally less reliable, likely because the training data wasn’t balanced enough. We also saw that the model sometimes gave unpredictable results, which we think is due to the incomplete and unbalanced dataset.

* **What We Would Do Differently with More Time/Resources:**
We would focus on making the model fairer by adding more images of people with darker skin tones and try different types of models to see if another approach might work better.

* **Additional Datasets or Techniques to Explore:**
To improve the model, we’d look for additional datasets that include a wider variety of skin tones, so the model can learn from a more diverse set of images. We’d also consider using pre-trained models, especially ones already trained for image analysis, and fine-tuning them for our task.

---

## **📄 References & Additional Resources**

[Medium – 7 Best Techniques To Improve The Accuracy of CNN W/O Overfitting](https://gurjeet333.medium.com/7-best-techniques-to-improve-the-accuracy-of-cnn-w-o-overfitting-6db06467182f)

---

### **👥 Team Members**

| Name | GitHub Handle | Contribution |
| ----- | ----- | ----- |
| Andersen Prince | @APrince26 | Contributed to building the CNN model and writing the GitHub README file |
| Dhriti Madireddy | @mdhritireddy7 | Contributed to building CNN model |
| Phuoc Uong | @cnrbd | Contributed to building CNN model |
| Ula Nguyen | @Uyenng | Contributed to building the CNN model and writing the GitHub README file  |
| Vanessa Pliego | @vpliego | Contributed to building the CNN model and writing the GitHub README file  |
| Yvette Roos | @yvette-m | Contributed to building CNN model |

Break Through Tech AI @MIT

January-March 2025
