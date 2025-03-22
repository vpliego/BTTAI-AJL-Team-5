# BTTAI-AJL-Team-5

## **🎯 Project Highlights**

**Example:**

* Built a \[insert model type\] using \[techniques used\] to solve \[Kaggle competition task\]
* Achieved an F1 score of \[insert score\] and a ranking of \[insert ranking out of participating teams\] on the final Kaggle Leaderboard
* Used \[explainability tool\] to interpret model decisions
* Implemented \[data preprocessing method\] to optimize results within compute constraints

🔗 [Equitable AI for Dermatology | Kaggle Competition Page](https://www.kaggle.com/competitions/bttai-ajl-2025/overview)

---
## **👩🏽‍💻 Setup & Execution**

**Provide step-by-step instructions so someone else can run your code and reproduce your results. Depending on your setup, include:**

* How to clone the repository
* How to install dependencies
* How to set up the environment
* * How to access the dataset(s)
* How to run the notebook or scripts

---
## **🏗️ Project Overview**

**Describe:**

* The Kaggle competition and its connection to the Break Through Tech AI Program
* The objective of the challenge
* The real-world significance of the problem and the potential impact of your work

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

**Describe:**

* The dataset(s) used (i.e., the data provided in Kaggle \+ any additional sources)
* Data exploration and preprocessing approaches
* Challenges and assumptions when working with the dataset(s)

**Potential visualizations to include:**

* Plots, charts, heatmaps, feature visualizations, sample dataset images
---
## **🧠 Model Development**

**Describe (as applicable):**

* Model(s) used (e.g., CNN with transfer learning, regression models)
* Feature selection and Hyperparameter tuning strategies
* Training setup (e.g., % of data for training/validation, evaluation metric, baseline performance)


**Methodology**: To meet our goals and objectives, we will be using a sequential Convolution Neural Network (CNN) since we will need our model to learn from the images in our data. To do this, we will be using tensorflow keras for importing and building our neural network. This is our optimal choice of modeling because of the many layers we can build on, allowing each layer to learn to detect the different features within an image which will be very useful in classifying skin conditions across the different features (i.e. skin color) of patients. 

---
## **📈 Results & Key Findings**

**Describe (as applicable):**

* Performance metrics (e.g., Kaggle Leaderboard score, F1-score)
* How your model performed overall
* How your model performed across different skin tones (AJL)
* Insights from evaluating model fairness (AJL)

**Potential visualizations to include:**

* Confusion matrix, precision-recall curve, feature importance plot, prediction distribution, outputs from fairness or explainability tools
---
## **🖼️ Impact Narrative**
**AJL challenge:**

As Dr. Randi mentioned in her challenge overview, “Through poetry, art, and storytelling, you can reach others who might not know enough to understand what’s happening with the machine learning model or data visualizations, but might still be heavily impacted by this kind of work.”
As you answer the questions below, consider using not only text, but also illustrations, annotated visualizations, poetry, or other creative techniques to make your work accessible to a wider audience.
Check out [this guide](https://drive.google.com/file/d/1kYKaVNR\_l7Abx2kebs3AdDi6TlPviC3q/view) from the Algorithmic Justice League for inspiration!

1. What steps did you take to address [model fairness](https://haas.berkeley.edu/wp-content/uploads/What-is-fairness_-EGAL2.pdf)? (e.g., leveraging data augmentation techniques to account for training dataset imbalances; using a validation set to assess model performance across different skin tones)
2. What broader impact could your work have?

---

## **🚀 Next Steps & Future Improvements**

**Address the following:**

* What are some of the limitations of your model?
* What would you do differently with more time/resources?
* What additional datasets or techniques would you explore?

---

## **📄 References & Additional Resources**

* Cite any relevant papers, articles, or tools used in your project

[Medium – 7 Best Techniques To Improve The Accuracy of CNN W/O Overfitting](https://gurjeet333.medium.com/7-best-techniques-to-improve-the-accuracy-of-cnn-w-o-overfitting-6db06467182f)

---

### **👥 Team Members**

| Name | GitHub Handle | Contribution |
| ----- | ----- | ----- |
| Andersen Prince | @x | Contributed to building CNN model |
| Dhriti Madireddy | @x | Contributed to building CNN model |
| Phuoc Uong | @x | Contributed to building CNN model |
| Ula Nguyen | @Uyenng | Contributed to building CNN model |
| Vanessa Pliego | @vpliego | Contributed to building CNN model |
| Yvette Roos | @yvette-m | Contributed to building CNN model |

January-March 2025
