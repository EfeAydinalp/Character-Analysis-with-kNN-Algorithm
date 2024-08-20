# Personality Classification with K-Nearest Neighbor Algorithm

This project implements a K-Nearest Neighbor (KNN) algorithm to classify different personality types based on the 16 Personality model. The classification is based on a dataset containing responses to personality test questions. The project also includes a variant of the algorithm, Weighted KNN, which adjusts the influence of neighbors based on their distance to the query point.

## Features
- **KNN Implementation:** Classifies personalities based on nearest neighbors.
- **Weighted KNN:** An optional weighted approach to improve classification by giving more weight to closer neighbors.
- **Performance Evaluation:** Computes accuracy, precision, and recall to evaluate the model’s performance.
- **Cross-Validation:** Uses 5-fold cross-validation to ensure reliable performance metrics.

## How to Run
1. Ensure all necessary Python packages are installed:
    - `pandas`
    - `numpy`
    - `matplotlib`
    - `random`

2. Download the personality classification dataset from the provided [Kaggle link](https://www.kaggle.com/datasets/anshulmehtakaggl/60k-responses-of-16-personalities-test-mbt).

3. Place the dataset in the working directory.

4. Run the Jupyter notebook (`Character Analysis with kNN Algorithm.ipynb`) in an environment that supports Jupyter.

## Dataset
- **Source:** 60,000 samples from a 16 Personality test.
- **Features:** 61 independent variables representing responses to questions, and 1 dependent variable representing personality type.
- **Preprocessing:** Drop the "Response Id" column and normalize features using min-max normalization.

## Testing
The implementation allows testing the model with various values of `k` (1, 3, 5, 7, 9) and includes the option to test both standard KNN and Weighted KNN. Results are evaluated using accuracy, precision, and recall metrics.

## Known Issues
- The current implementation may struggle with performance when dealing with noisy data or outliers.
- Weighted KNN might overfit in some scenarios where `k` is not optimally chosen.

## Future Improvements
- Implement more advanced distance metrics to see if classification can be improved.
- Enhance error analysis by providing more detailed explanations for misclassifications.


USEFUL LINKS:  For accuracy, recall and precision measurement.


https://stats.stackexchange.com/questions/51296/how-do-you-calculate-precision-and-recall-for-multiclass-classification-using-co/51301#51301

https://datascience.stackexchange.com/questions/15989/micro-average-vs-macro-average-performance-in-a-multiclass-classification-settin/24051#24051

