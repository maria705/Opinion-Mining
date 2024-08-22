# Opinion-Mining
Opinion Mining of Product Reviews

# Opinion Mining and Aspect-Based Sentiment Analysis

This repository contains an implementation of opinion mining and aspect-based sentiment analysis using deep learning techniques. The code performs opinion phrase extraction, aspect prediction, and product prediction from customer reviews.

## Dataset

The dataset used in this project is stored in a CSV file named `mm.csv`. It contains the following columns:
- `Reviews`: The text of the customer reviews.
- `Opinion_Phrases`: The opinion phrases present in each review.
- `Aspect`: The aspect associated with each review.
- `Product`: The product associated with each review.


## Usage

1. Make sure you have the required dependencies installed.

2. Place the `mm.csv` file in the appropriate directory.

3. Run the code file `opinion_mining.py` to perform opinion mining and aspect-based sentiment analysis:
   ```
   python opinion_mining.py
   ```

4. The code will preprocess the data, create a vocabulary, and convert the reviews into numerical representations using word embeddings.

5. It will then create a dataset with word-level labels for opinion phrases and convert the labels into numerical representations.

6. The code defines a deep learning model architecture using a bidirectional LSTM network.

7. K-fold cross-validation is performed to train and evaluate the model. The evaluation metrics (accuracy, precision, recall, F1-score) are calculated for each fold.

8. The average metrics across all folds are printed, indicating the overall performance of the model.

9. Aspect and product prediction are performed using TF-IDF vectorization and linear SVM classifiers.

10. The code provides inference functions to predict the opinion phrase, aspect, and product for a given review.

## Results

The code outputs the following:
- Confusion matrix plot for each fold, visualizing the model's performance in classifying opinion phrases.
- Training vs validation loss and accuracy plots for each fold, showing the model's learning progress.
- Average accuracy, precision, recall, and F1-score across all folds, indicating the overall performance of the model.

