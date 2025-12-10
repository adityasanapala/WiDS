# Week 1 - Foundations of NLP

## Concepts

### 1. What is NLP? Tokens, Types, Corpora

Video Resource: [What are Word Embeddings?](https://www.youtube.com/watch?v=wgfSDrqYMJ4)

Word Embeddings and Word2Vec - https://www.youtube.com/watch?v=viZrOnJclY0
One-Hot, Label, Target and K-Fold Target Encoding - https://www.youtube.com/watch?v=589nCGeWG1w

### 2. Text Preprocessing

- [tokenization](https://youtu.be/fNxaJsNG3-s?si=giRDIRu-1Y7KWSlQ)

- [stemming vs lemmatization](https://youtu.be/HHAilAC3cXw?si=PB4H-PnwdvU_CfJI)

- [stopword removal](https://youtu.be/vUPAOU2NPls?si=3zTpPSHUD8_o3Jao)

- [n-grams](https://youtu.be/nZromH6F7R0?si=gUS_6gQOJ25PIBqK)

### 3. Basic ML for NLP (Bag-of-Words, TF-IDF)

(1)BOW:
Basic thought process: https://www.youtube.com/watch?v=Yt1Sw6yWjlw
The actual code and extra stuff: https://www.youtube.com/watch?v=8Mlc4-3tgzc

(2)TF-IDF:
https://www.youtube.com/playlist?list=PLy0R06Fv9ZSIHjFje2d53WztJeNjHW0zT

### 4. Evaluation metrics: accuracy, F1, BLEU (overview)

These apply when the output is a label.

- Accuracy
Fraction of total correct predictions.
Works only when data is balanced. Misleading for imbalance.

- Precision
Of all predicted positives, how many were truly positive.
Use when false positives are costly.

- Recall
Of all actual positives, how many did the model find.
Use when false negatives are costly.

- F1 Score
Harmonic mean of Precision and Recall.
One number summarizing both.
Best when classes are imbalanced or both errors matter.

- In simple terms:
  Accuracy = overall score
  Precision = trust in positive predictions
  Recall = ability to capture all positives
  F1 = balance between the two

BLEU (used for machine translation / text generation):

BLEU is used when output is generated text, not labels.
  Compares n-gram overlap between model output and reference text.
  Includes brevity penalty so very short sentences don’t get high scores.
  Good for machine translation, basic generation tasks.
  Weak when meaning is similar but wording differs (synonyms, paraphrasing).

Resources:

(1) Precision, Recall, and F1 Explained: 
- https://medium.com/@isachinkamal/evaluating-nlp-models-precision-recall-and-f1-explained-467e8940391a
- Just a short go through(formulas>>):
  https://fiveable.me/lists/common-nlp-evaluation-metrics?utm_source=chatgpt.com
  https://fiveable.me/natural-language-processing/unit-2/evaluation-metrics-text-classification/study-guide/TgMlFZUwVbDvWPo6?utm_source=chatgpt.com

(2) BLEU:
- https://youtu.be/25kutmqou6o
- https://www.geeksforgeeks.org/nlp/understanding-bleu-and-rouge-score-for-nlp-evaluation/?utm_source=chatgpt.com
- Just a short go through:
  https://www.scaler.com/topics/nlp/bleu-score-in-nlp/?utm_source=chatgpt.com

### 5. Regex - https://www.youtube.com/watch?v=lK9gx4q_vfI

## Coding Tasks

- Implement tokenization & stemming using Python + NLTK / spaCy

- Build a TF-IDF text classifier for sentiment (IMDb or SST-2)

- Explore Hugging Face datasets:
Video: https://www.youtube.com/watch?v=-S20nblUuNw
Documentation: https://www.geeksforgeeks.org/artificial-intelligence/hugging-face-dataset-hub/?utm_source=chatgpt.com

## Resources

- [NLTK book (free)](https://www.nltk.org/book/)

- [spaCy course (free)](https://course.spacy.io/en/)
