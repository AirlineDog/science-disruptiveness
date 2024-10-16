## Predicting Scientific Paper Disruptiveness

**Introduction**

This project aims to predict the disruptiveness of scientific papers using machine learning techniques. Disruptiveness is measured using the CD5 index, which quantifies how likely a paper's citations are to cite the paper's own references. A higher CD5 index indicates a more disruptive paper.

**Dataset**

The dataset used is derived from the Alexandria3k package and contains a 1% sample of CrossRef available publications with abstracts.

**Methodology**

1. **Data Preprocessing:**
   * Remove HTML tags, numbers, and special characters from abstracts and titles.
   * Lemmatize words in abstracts and titles.

2. **Feature Engineering:**
   * Create additional features based on the dataset, such as vocabulary uniqueness, number of authors and references, average reference year, and author affiliations.

3. **Model Training:**
   * Train various machine learning models, including:
     * Decision Tree Regressor
     * XGBoost and LightGBM Regressor
     * Voting and Stacking Ensemble methods
     * Neural Network
   * Use cross-validation to evaluate model performance and tune hyperparameters.

4. **Evaluation:**
   * Evaluate models using the mean absolute error metric.
   * Compare the performance of different models to identify the best-performing one.

**Results**

The results indicate that while the models can predict disruptiveness to some extent, the accuracy is limited. This could be due to factors such as the complexity of the task, the limited dataset size, and the potential limitations of the features used.

**Future Work**

Future work could explore the following:

* Incorporate additional features, such as semantic analysis of text.
* Experiment with different machine learning algorithms and techniques.
* Collect a larger and more diverse dataset.
* Investigate the impact of linguistic changes on disruptiveness.

