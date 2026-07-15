# Module 02 — Machine Learning Fundamentals

## Learning Objectives

By the end of this module students will:

- Understand what Machine Learning is and how it differs from traditional programming
- Identify the three types of machine learning
- Interpret basic ML concepts: features, labels, training, testing
- Recognise common ML algorithms and their use cases

---

## Topics Covered

### 1. What is Machine Learning?

Machine Learning is a subset of AI where systems learn patterns from data and improve their performance without being explicitly programmed for every scenario. Instead of writing rules, you give the system examples, and it figures out the rules itself. A traditional spam filter might use hand-written rules ("block emails with the word 'free money'"). An ML spam filter learns to identify spam by studying thousands of examples of spam and legitimate emails.

### 2. Traditional Programming vs ML

In traditional programming: you provide **data + rules** → the program produces **outputs**.
In Machine Learning: you provide **data + outputs** → the system learns the **rules**.

This inversion is what makes ML powerful for problems where the rules are too complex or numerous to write by hand — recognising faces, understanding speech, predicting customer behaviour.

### 3. Supervised Learning

Supervised learning trains on **labelled data** — every training example has a known correct answer (the label). The model learns to map inputs to outputs by seeing many examples.

**Common tasks:**
- **Classification:** Assign inputs to categories (spam/not spam, disease/healthy, fraud/legitimate)
- **Regression:** Predict a continuous value (house price, temperature, sales forecast)

**Examples:** Email spam detection, credit scoring, medical diagnosis, demand forecasting.

### 4. Unsupervised Learning

Unsupervised learning finds patterns in **unlabelled data** — no correct answers are provided. The model discovers structure on its own.

**Common tasks:**
- **Clustering:** Group similar items together (K-Means, DBSCAN)
- **Dimensionality reduction:** Compress data while preserving structure (PCA)
- **Anomaly detection:** Identify unusual data points

**Examples:** Customer segmentation, topic modelling in documents, anomaly detection in network traffic.

### 5. Reinforcement Learning

Reinforcement learning trains an **agent** that learns by taking actions in an environment and receiving **rewards** or **penalties**. There is no dataset — the agent learns through trial and error.

**Examples:** Game-playing AI (AlphaGo, chess engines), robotics control, recommendation systems, self-driving car navigation.

### 6. Key Concepts: Features, Labels, Training, Testing, Overfitting

**Feature:** An individual measurable property used as model input (e.g., "number of bedrooms" for house price prediction).
**Label:** The correct answer for a training example (e.g., the actual house price).
**Training set:** Data used to train the model — the model sees and learns from this data.
**Test set:** Data the model has never seen — used to evaluate real-world performance.
**Overfitting:** When a model memorises training data rather than learning general patterns, performing well on training but poorly on new data.
**Underfitting:** When a model is too simple to capture the underlying patterns, performing poorly on both training and new data.

### 7. Common Algorithms Overview

**Linear Regression:** Predicts a continuous output as a weighted sum of inputs. Simple, interpretable, fast.
**Logistic Regression:** Despite the name, used for binary classification. Predicts probability of class membership.
**Decision Trees:** Tree-structured models that split data based on feature thresholds. Highly interpretable.
**Random Forest:** An ensemble of decision trees that votes on predictions. More accurate and robust than a single tree.
**K-Means Clustering:** Partitions data into K groups by minimising within-group distance. Requires choosing K in advance.
**K-Nearest Neighbours (KNN):** Classifies a new point based on the majority class of its K nearest neighbours in the training data.

### 8. ML in Practice — Real Industry Examples

- **Healthcare:** Predicting patient readmission risk from medical records
- **Retail:** Forecasting product demand to optimise inventory
- **Finance:** Detecting credit card fraud in real time
- **HR:** Screening resumes (controversial — see Module 08 for bias implications)
- **Agriculture:** Predicting crop yield from satellite imagery and weather data

---

## Demonstrations

- Training a simple image classifier in Google Teachable Machine (live, no code)
- Visualising decision boundaries interactively
- K-Means clustering demo on a 2D dataset

## Hands-on Activities

- Build an image classifier using Teachable Machine — train it on hand gestures
- Explore a dataset on Kaggle and identify features vs labels
- Predict outcomes using a simple regression tool

## Assignment

Using a dataset of your choice, write a 300-word analysis describing: the features and label, which type of ML applies, what real-world decision it could support, and one potential bias risk. See `../../assessments/assignments/README.md` for full brief.

## Additional Resources

- [Google Teachable Machine](https://teachablemachine.withgoogle.com/)
- [Kaggle Learn — Intro to ML](https://www.kaggle.com/learn/intro-to-machine-learning)
- [ML for Beginners — Microsoft GitHub](https://github.com/microsoft/ML-For-Beginners)

---

*Previous: [Module 01 — Introduction to AI](../01-Introduction-to-AI/README.md)  |  Next: [Module 03 — Deep Learning & Neural Networks](../03-Deep-Learning-Neural-Networks/README.md)*
