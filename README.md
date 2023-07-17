[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/rBRzfPCb)

# Group Members
1. Bless Ziamah - 10922782
2. Vera Achiaa Owusu - 10923847
3. Herbert Ansah Akrofi - 10923111


project_report = '''
## Project Report: Predicting Words Influencing Sentiment in Tweet Text

### Introduction:
The goal of this project is to predict words that heavily influence the sentiment of tweet text. By identifying these influential words, we aim to gain insights into the language patterns and expressions that strongly contribute to the sentiment expressed in tweets. The project utilizes techniques such as data preprocessing, word counting, frequency comparison, and Jaccard similarity to achieve the desired prediction.

### Procedure:
1. **Data Preparation:**
    - The project starts with data preparation by loading the necessary datasets, such as `X_train`, `X_test`, `y_train`, and `y_test`, which contain the tweet text, sentiment labels, and selected text (ground truth).

2. **Preprocessing and Word Counting:**
    - To handle the textual data, a preprocessing step is performed using the `preprocess_tweet_text` function to clean and normalize the text.
    - The `get_word_count` function is used to calculate the frequency of each word in the tweet text. This function preprocesses the text, splits it into words, and then counts the occurrence of each word.

3. **Frequency Comparison:**
    - The `freq_comparison` function is employed to compare word frequencies between a parent column (tweet text) and a child column (selected text). This function determines words that are present in the parent column but not in the child column, or words that have significantly higher frequencies in the parent column compared to the child column.

4. **Predicting Selected Words:**
    - The `predict` function is created to predict the selected words in a given tweet text based on the specified sentiment. It preprocesses the input sentence, filters out words present in the `remove_list` (obtained from the frequency comparison), and returns the selected words.

5. **Jaccard Similarity Calculation:**
    - The `jaccard` function calculates the Jaccard similarity coefficient between two strings. It converts the strings to lowercase, splits them into words, finds the intersection of words, and computes the Jaccard similarity coefficient.

6. **Evaluation and Reporting:**
    - The project evaluates the predictions by comparing them with the ground truth selected text. It calculates the Jaccard similarity coefficient between the predicted selected words and the actual selected words.
    - The mean of the Jaccard similarity coefficients is then computed to measure the overall accuracy of the predictions.

### Conclusion:
The project successfully accomplishes the objective of predicting words that heavily influence the sentiment of tweet text. By applying techniques such as data preprocessing, word counting, frequency comparison, and Jaccard similarity, it provides insights into the influential language patterns and expressions that contribute to the sentiment expressed in tweets. The evaluation of predictions using Jaccard similarity ensures the accuracy and reliability of the results. The findings from this project can be further utilized for sentiment analysis, opinion mining, and understanding the impact of specific words on sentiment in social media data.


