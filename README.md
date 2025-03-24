# BTTAI-AJL-Team-5

## **🎯 Project Highlights**

* Built a CNN model using ReLU as our activation function to introduce non-linearity to the network in order to address the Algorithmic Justice League’s goal of bringing inclusivity to model building. The specific task from AJL seeks to address issues within healthcare and dermatology that currently leave individuals of color without accurate diagnoses because of faulty systems. In the model that we build, we aim to produce accurate results for individuals of a wide range of skin tones and minimize the bias that we are currently seeing within the healthcare industry.  
* Achieved an F1/accuracy score of 31%.
* Implemented data encoding and created image generators to load images and labels properly to optimize results within computing constraints

🔗 [Equitable AI for Dermatology | Kaggle Competition Page](https://www.kaggle.com/competitions/bttai-ajl-2025/overview)

---
## **👩🏽‍💻 Setup & Execution**

### How to clone the repository
Follow [this instruction](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) 

* How to access the dataset(s)
  
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

**Describe (as applicable):**

* Model(s) used (e.g., CNN with transfer learning, regression models)
* Feature selection and Hyperparameter tuning strategies
* Training setup (e.g., % of data for training/validation, evaluation metric, baseline performance)


We use a sequential Convolution Neural Network (CNN) to learn from the images in our data. To do this, we will be using tensorflow keras for importing and building our neural network. This is our optimal choice of modeling because of the many layers we can build on, allowing each layer to learn to detect the different features within an image which will be very useful in classifying skin conditions across the different features (i.e. skin color) of patients.

---
## **📈 Results & Key Findings**

**Describe (as applicable):**

* Performance metrics (e.g., Kaggle Leaderboard score, F1-score)
* How your model performed overall
* How your model performed across different skin tones (AJL)
* Insights from evaluating model fairness (AJL)

Our model achieved an F1 score of 31% on the validation set and ranked 37 on the Kaggle leaderboard. We used F1 score as the main metric because it balances precision and recall, which felt more important than just accuracy, especially for this task where false negatives could have a real world impact.

The model did okay. It didn’t get everything right, but it learned patterns and was better than just guessing. We tried different models, and the one we used at the end gave me the best results, even if the score wasn’t super high.

When we checked how it worked for different skin tones, we saw it did better on lighter skin and not as well on darker skin. That means it wasn’t totally fair and didn’t treat everyone the same.

Considering fairness got me to consider more about how models can fail in a variety of ways. Just because it performs fine overall doesn't imply that it's fine for everybody. If we could continue to work on it, we'd attempt to correct the bias by incorporating more examples of dark skin so that it might learn better. We would also test it on other groups to ensure that it is equitable for all, not only the most well-represented in the training data. This is necessary because an unfair model could result in individuals being discriminated against or treated unequally in real-world applications, which is unacceptable.

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

We looked at the model's performance on various skin tones to evaluate its fairness. The model performed better on light skin tones and relatively poorly on dark skin tones, so we concluded that there was an issue. Thus, we thought about adding more photos of individuals with darker skin tones to balance this out. We even thought about changing some of the pictures, like making some lighter or darker, so that the model would get more kinds of photos to train on. We did not get a chance to do all that, but we learned why we should.

If this kind of model were to be used in real-world applications, it could potentially help with something like image analysis or maybe even helping people. However, if the model is seen as unfair, then it could also cause more damage than the benefits it may be intended to have. Our project has shown that it is not enough for a model to simply be decent. It needs to work well for everyone. 

---

## **🚀 Next Steps & Future Improvements**

**Address the following:**

* What are some of the limitations of your model?
* What would you do differently with more time/resources?
* What additional datasets or techniques would you explore?

Our model did not always produce correct results. It struggled with darker skin colors and was less accurate. It gave unpredictable results at times, which we blame on the incompleteness and lack of balance of the training data.

If we had more time, we'd try to make the model fairer by adding more pictures of people with darker skin. We would also try different types of models to see if any worked better. And we would clean up the data more so it's easier for the model to learn from.

We would find more datasets with all sorts of skin colors. We'd also use techniques like changing the images size or changing the brightness to help the model practice with differently looking photos. 

---

## **📄 References & Additional Resources**

* Cite any relevant papers, articles, or tools used in your project

[Medium – 7 Best Techniques To Improve The Accuracy of CNN W/O Overfitting](https://gurjeet333.medium.com/7-best-techniques-to-improve-the-accuracy-of-cnn-w-o-overfitting-6db06467182f)

---

### **👥 Team Members**

| Name | GitHub Handle | Contribution |
| ----- | ----- | ----- |
| Andersen Prince | @APrince26 | Contributed to building CNN model |
| Dhriti Madireddy | @x | Contributed to building CNN model |
| Phuoc Uong | @x | Contributed to building CNN model |
| Ula Nguyen | @Uyenng | Contributed to building CNN model |
| Vanessa Pliego | @vpliego | Contributed to building CNN model |
| Yvette Roos | @yvette-m | Contributed to building CNN model |

January-March 2025
