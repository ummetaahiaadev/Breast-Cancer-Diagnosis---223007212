This project predicts breast cancer diagnosis using:
- K-Nearest Neighbors (KNN)— Supervised classification
- K-Means Clustering— Unsupervised grouping

This assignment follows the exact instructions provided by the instructor.

Objectives:
- Classify breast cancer tumors into:
  - Malignant (M → 1)
  - Benign (B → 0)
- Apply:
  - Min-Max Normalization**
  - K-Means Clustering (k = 2)
  - KNN Classification (k = 5)
- Evaluate using:
  - Accuracy
  - Precision
  - Recall
  - F1-score

Columns include measurements such as:
- radius
- texture
- smoothness
- concavity
- fractal dimension  
and many more (total: 30+ features).

The dataset also contains:
- diagnosis (M/B)
- id
- Unnamed: 32 (empty column)

Preprocessing Steps:
1. Dropped unnecessary columns 
   - `id`  
   - `Unnamed: 32`  

2. Encoded diagnosis column
   - `M → 1`  
   - `B → 0`

3. Applied Min-Max Normalization 
   Scaling each feature to range [0, 1].

4. Train-test split  
   - 80% training  
   - 20% testing  

K-Means Clustering:
- Applied K-Means with k = 2
- Cluster labels were used only for observation (not model training)
- Helps visualize how malignant and benign data points naturally group

KNN Classification:
- Trained **KNN model with k = 5
- Used scaled features for training and testing

Model Evaluation (KNN Results):

| Metric        | Value |
|---------------|--------|
| **Accuracy**  | 0.9649 |
| **Precision** | 0.9535 |
| **Recall**    | 0.9535 |
| **F1-score**  | 0.9535 |
The model performs extremely well on the test dataset.
