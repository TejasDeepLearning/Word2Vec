# Word2Vec Training and Evaluation
This repository contains code for training and evaluating a Word2Vec model using the Skip-gram architecture. The Word2Vec model is a popular technique in Natural Language Processing (NLP) for learning word embeddings, which capture the semantic and syntactic relationships between words.

## Installation
To use this code, please follow these steps:

1. Clone the repository: git clone https://github.com/your-username/word2vec.git
2. Install the required dependencies: pip install -r requirements.txt

## Usage
### Training the Word2Vec Model
To train the Word2Vec model, execute the following command: 

`python train_model.py savedir`

Replace savedir with the directory where you want to save the trained model.

### Evaluating the Word2Vec Model
To evaluate the Word2Vec model, execute the following command:

`python test_model.py savedir`

Replace savedir with the directory where the trained model is saved.

## Example Analogy Tests
The test_model.py script includes several analogy tests to demonstrate the capabilities of the trained Word2Vec model. Here are some example analogy tests:

1. king - man = queen - woman
2. miami - florida = dallas - texas
3. einstein - scientist = picasso - painter
4. man - woman = he - she

These tests aim to find words that have similar relationships as the provided analogy. The results of the analogy tests will be printed to the console.

## Model Persistence
The trained Word2Vec model can be saved to disk for future use. The model includes the word-to-index mapping (word2idx), the input-to-hidden weights (W), and the hidden-to-output weights (V).

To load a saved model, use the following code:

`word2idx, W, V = load_model('savedir')`

Replace 'savedir' with the directory where the model is saved.

## Acknowledgments
This implementation is based on the course "Natural Language Processing with Deep Learning in Python" by Lazy Programmer Inc. Special thanks to the instructor for providing the code and materials.
