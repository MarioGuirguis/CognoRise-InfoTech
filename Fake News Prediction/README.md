# Fake News Prediction

This project aims to build a machine learning model to detect fake news using the **Fake News Prediction Dataset**. The dataset contains both real and fake news articles, categorized by labels, and provides a foundation for creating a predictive model to identify misinformation.

## Steps in the Code

1. **Data Loading and Preprocessing**:
   - The dataset is loaded, and the `Title` and `Text` columns are concatenated to form a unified text feature.
   - Text data is preprocessed using **text to sequence** conversion, which transforms the text into a sequence of integers where each integer represents a word’s index in the tokenizer's vocabulary.
   - **Padding** is applied to the sequences to ensure uniform input length for the model.

2. **Model Architecture**:
   - A **Neural Network** model based on **LSTM (Long Short-Term Memory)** is built to classify the news articles. The key layers include:
     - **Embedding Layer**: Converts the input sequence of word indices into dense vectors of fixed size, capturing the semantic relationship between words.
     - **LSTM Layer**: A recurrent layer used to capture long-term dependencies in the text.
     - **Dropout Layers**: Added to reduce overfitting by randomly dropping units during training.
     - **Dense Output Layer with Sigmoid Activation**: The final layer outputs a probability score for binary classification (real or fake).

3. **Model Training**:
   - The model is trained using the **binary cross-entropy loss function** and the **Adadelta optimizer**.
   - The training is conducted over multiple epochs, with accuracy tracked on both the training and validation sets.

4. **Model Evaluation**:
   - After training, the model's performance is evaluated using accuracy on the test set. The final model achieves an accuracy of **87.6%** on the test data.
