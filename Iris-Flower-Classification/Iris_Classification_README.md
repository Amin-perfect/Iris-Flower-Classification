# Iris Species Classification

## The Question Behind the Project
Can a machine tell three flower species apart using nothing but four numbers — sepal length, sepal width, petal length, and petal width? This project answers that question by walking through a complete classification pipeline, from raw measurements to predicted species.

## Why Iris?
The Iris dataset is one of the oldest and most studied datasets in machine learning, and for good reason — it's small enough to fully understand by eye, yet rich enough to teach the fundamentals of classification: feature separability, decision boundaries, and model evaluation. I used it to build a solid foundation in multi-class classification before moving to messier, real-world datasets.

## What the Model Learns
Given four flower measurements, the model predicts whether a sample is:
- *Iris-setosa*
- *Iris-versicolor*
- *Iris-virginica*

## How It Works
- **Visual exploration first** — before training anything, I used pairplots to see how the species separate visually across feature pairs. This step mattered: it showed that petal measurements separate the classes far more cleanly than sepal measurements.
- **Correlation heatmap** — confirmed which features carried the most predictive signal.
- **Train-test split** — held out a portion of the data to test generalization rather than memorization.
- **Logistic Regression** — trained as a multi-class classifier on the four features.
- **Evaluation** — measured prediction accuracy on the unseen test set.

## Result
The model scored a perfect 1.0 accuracy on the test set. This isn't a sign of an exceptional model — it reflects a well-known property of this dataset: the three species, especially *setosa*, are almost linearly separable using petal measurements alone. A small, clean dataset like this can reach perfect test accuracy without overfitting, which is part of what makes it such a good teaching dataset in the first place.

## What I'd Improve Next
Testing the same pipeline on a noisier, larger classification dataset to see how the model behaves when classes aren't as cleanly separable — and comparing Logistic Regression against a decision tree or KNN classifier on that harder case.

## Tech Stack
Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn · Jupyter Notebook

## Author
Amin (Mr. PerfecT) — BSCS Student | Aspiring Data Scientist & AI Developer
