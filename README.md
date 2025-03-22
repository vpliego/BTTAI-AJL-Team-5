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

This project is a Kaggle competition presented by Break Through Tech and the [Algorithmic Justice League (AJL)](https://www.ajl.org/about). Break Through Tech AI Fellows from the Virtual, Boston (MIT), and Los Angeles (UCLA) programs participated in this Kaggle competition.

With the rise of AI over the past few years, tasks within diverse fields, like in healthcare, that once required extensive human labor have now been simplified with models that can easily and quickly classify large amounts of data. However, the data that has been used for these models thus far have been filled with problematic patterns of bias, unrepresentative of a wide range of individuals, and overall lacking the inclusivity of different identities. As a result, we see models that succeed for certain groups more than others and at the same time continue discriminating against marginalized and vulnerable groups-- these groups usually being low-income communities of color. 

The Algorithmic Justice League (AJL) is an organization that works to combat the social implications and harms around AI as the one described earlier. In this project, we will work to build a model that classifies skin conditions across diverse skin tones, as this is currently a challenge being seen within dermatology and the models being used for diagnoses. It is imperative that our project challenges the current models being used because of the potential misdiagnosing and harm being done to vulnerable communities. Therefore, it is our role and responsibility as data and machine learning engineers to ethically combat the current models being used in dermatology by training a model that learns from a diverse and inclusive set of data. In doing so, we aim to limit any biases and poor models that are currently misdiagnosing marginalized patients with skin conditions.

**Goals**: Our main goal with this project is to build an ethically responsible model that can be used by a diverse set of people. As mentioned in our project overview, current models being used in the dermatology field fail to classify patients of diverse skin tones, which results in misdiagnosis and delayed treatment which runs the possibility of being fatal or detrimental to the patient's life. Therefore, with our model, we hope to address diverse groups of people by using more representative data and train a model with high accuracy levels to improve the current healthcare experience of vulnerable communities.  

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
| Dhriti Madireddy | @x | x |
| Phuoc Uong | @x | x |
| Ula Nguyen | @Uyenng | Contributed to building CNN model |
| Vanessa Pliego | @vpliego | Contributed to building CNN model |
| Yvette Roos | @yvette-m | x |

January-March 2025
