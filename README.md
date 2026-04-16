# Transformer Text Classification on Reuters-46

Encoder-only Transformer (TensorFlow/Keras) for 46-class news classification. Compared with RNN, LSTM, GRU, and bidirectional variants.

## Results

| Model | Test Accuracy | Weighted F1 |
|-------|---------------|-------------|
| Transformer (3 layers) | **0.7502** | **0.7409** |
| Transformer (5 layers) | 0.7315 | 0.7223 |
| Transformer (7 layers) | 0.6883 | 0.6905 |
| BiLSTM (best baseline) | – | 0.6894 |

## Key Features

- Stackable encoder blocks (3/5/7 layers) with variable feed-forward dimensions
- Custom 'TokenAndPositionEmbedding' and 'TransformerBlock' layers
- Controlled 10‑epoch experiments with confusion matrices and classification reports
