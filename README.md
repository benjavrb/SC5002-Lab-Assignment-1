# SC5002-Lab-Assignment-1
SC5002 Lab Assignment 1
Course: SC5002 Artificial Intelligence Fundamentals & Applications
Student: James Benjamin Burnias
Project Overview
This project explores classical AI search algorithms and applied machine learning. Part 1 compares Breadth-First Search (BFS) and A* Search on a directed graph and uses A* to solve an 8-puzzle. Part 2 uses the California Housing dataset to compare Linear Regression with Ridge Regression at different regularization strengths.
Part 1: Search Algorithms
- BFS: Found the path S → F → G, with two edges and total cost 9.
- A:* Found the lower-cost path S → B → D → G, with total cost 7.
- 8-puzzle: Using the number of misplaced tiles as the heuristic, the solution required five blank-tile moves: Up → Up → Left → Down → Right.
Part 2: Machine Learning
The notebook samples 1,000 records from the California Housing dataset (random state 42), uses eight numerical features to predict MedHouseVal, standardizes the features with StandardScaler, and evaluates Linear Regression and Ridge Regression with 5-fold cross-validation.
Model	Alpha	Mean 5-fold R²
Linear Regression	N/A	0.6457
Ridge Regression	0.1	0.6457
Ridge Regression	10.0	0.6443
Ridge Regression	1000.0	0.3574


The much lower R² score at alpha = 1000 suggests that excessive regularization causes underfitting in this experiment.
How to Run
1. Open the .ipynb notebook in Google Colab.
2. Run the notebook cells in order. The notebook uses Python, NumPy, pandas, Matplotlib, and scikit-learn.
3. Review the printed first five dataset rows, cross-validation R² scores, and performance comparison bar chart.
4. An internet connection may be required when the California Housing dataset is downloaded for the first time.
Use of Generative AI
Generative AI was used to explain admissible heuristics, check manual A* puzzle calculations, identify dataset features, and interpret regression and regularization results. The report includes the prompting logs and reflections.
Submission
This repository contains the machine-learning Colab notebook. The separate PDF report contains the search calculations, AI prompting logs, and analysis; a five-minute presentation summarizes the findings.
