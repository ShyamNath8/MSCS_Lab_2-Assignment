# MSCS_Lab_2-Assignment
Lab 2: K-Nearest Neighbors (KNN) vs Radius Neighbors (RNN) Classifiers using the Wine Dataset

Purpose of the Lab
The purpose of this lab is to explore and compare the performance of K-Nearest Neighbors (KNN) and Radius Neighbors (RNN) classifiers using the Wine dataset from the `sklearn` Python library. The lab demonstrates how different parameter values (k for KNN and radius for RNN) influence model accuracy. This hands-on analysis helps build an understanding of how to select suitable values to improve classification performance.

---

Key Insights

-KNN consistently performed well, with the highest accuracy observed at `k = 5` and `k = 11`.
-RNN accuracy was highly sensitive to the choice of radius. Small radius values often resulted in low accuracy or failure to make predictions due to no neighbors being found.
-KNN was more stable across tested values, while RNN required precise tuning to perform adequately.
- In dense and well-distributed datasets like Wine, KNN is a more reliable model choice.

---

Challenges and Decisions

-Selecting effective radius values for RNN was challenging. Some values led to prediction failures (no neighbors), so the `outlier_label=-1` parameter was added to handle such cases.
-Plotting accuracy trends helped visually identify optimal parameter values for both classifiers.
-Choosing `stratify=y` during data splitting helped maintain class balance between the training and test sets.

---

Files Included
- Lab2_KNN_RNN_Wine.ipynb – The main Jupyter Notebook containing the code, outputs, and visualizations.
- Assignment Screenshots and Discussion -File showing the comparison and instances of using KNN and RNN
- README.md – This file summarizing the lab purpose, insights, and key decisions.

---

Technologies Used
- Python
- Jupyter Notebook
- scikit-learn
- pandas
- matplotlib


