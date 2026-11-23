**Original repo date:** 24.01.2022 – 20.05.2022

---

# Classification-Mushrooms
Classifying mushrooms as **edible** or **poisonous** with the **K-Nearest Neighbors (KNN)** algorithm.

[Notebook with step-by-step explanations (in Turkish)](Classification%20KNN.ipynb)
<br>
[Code only](KNNMushrooms.py)

## Dataset

[mushrooms.csv](mushrooms.csv) contains 8,124 mushrooms described by 22 categorical features, such as cap shape, color, odor and habitat. The `class` column shows whether the mushroom is edible (`e`, 4,208 samples) or poisonous (`p`, 3,916 samples).

## Steps

1. Converting the categorical (letter) values to numbers with `LabelEncoder`
2. Creating dummy columns with `OneHotEncoder`
3. A 75% / 25% train-test split
4. Training a `KNeighborsClassifier` with 10 neighbors and the Minkowski (Euclidean) distance
5. Evaluating the predictions with a confusion matrix and 10-fold cross-validation
