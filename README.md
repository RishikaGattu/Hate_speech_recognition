# Hate_speech_recognition
Model Performance Summary
Our project evaluated the performance of several deep learning models for classifying text into three categories. Below is a detailed comparison of their results:

GRU (Gated Recurrent Unit)
Test Accuracy: 94.15%

Highlights:

Achieved the highest overall accuracy.

Demonstrated faster convergence and efficient handling of sequential data.

Bidirectional architecture enabled it to capture context from both past and future word sequences.

Balanced precision and recall, making it suitable for imbalanced datasets.

Ideal for real-world content moderation systems.

FFNN (Feedforward Neural Network)
Test Accuracy: 93.73%

Highlights:

Performed well on the dominant class ("offensive language").

Struggled with the minority class ("hate speech") due to its inability to model sequence or context.

Relied on TF-IDF or static embeddings, lacking understanding of word order or contextual flow.

Resulted in a lower macro-average F1-score, revealing bias toward majority class.

LSTM (Long Short-Term Memory)
Test Accuracy: 88.44%

Highlights:

Good at retaining long-term dependencies.

Captured semantic relationships across word sequences.

Required longer training time and careful regularization to avoid overfitting.

CNN (Convolutional Neural Network)
Test Accuracy: 88.36%

Highlights:

Excellent at identifying local patterns and n-grams such as offensive phrases.

Lacked capacity for long-range contextual understanding.

Less effective at detecting subtle or implicit hate speech.

Conclusion
While FFNN offered fast and reasonably accurate predictions, it lacked class sensitivity.

CNN and LSTM added value in different aspects: pattern detection and contextual modeling.

GRU emerged as the best-performing model, offering the optimal balance between:

Accuracy

Contextual understanding

Training efficiency

Robustness against overfitting
