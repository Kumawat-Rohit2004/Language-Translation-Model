## 📌 Small-Scale ChatGPT Model for Language Translation  

This project demonstrates how to build a **small-scale ChatGPT-like model** for **English → French translation** using TensorFlow. The implementation follows the Transformer encoder-decoder architecture and includes custom components for training and evaluation.  

### 🔑 Key Steps  

1. **Data Gathering & Preprocessing**  
   - Used the French-English dataset (`fra-eng`) from TensorFlow.  
   - Normalized text, added start/end tokens, and serialized preprocessed pairs.  

2. **Data Transformation & Vectorization**  
   - Applied `TextVectorization` for English & French.  
   - Created TensorFlow datasets for training and testing.  

3. **Positional Embedding**  
   - Implemented sinusoidal positional encoding.  
   - Built a custom `PositionalEmbedding` layer for sequence order understanding.  

4. **Neural Network Components**  
   - **Self-Attention**: Captures dependencies within a sequence.  
   - **Cross-Attention**: Connects encoder and decoder contexts.  
   - **Feed-Forward Layers**: Dense transformations with normalization.  

5. **Encoder-Decoder Transformer**  
   - Built encoder & decoder stacks with multi-head attention.  
   - Combined into a Transformer model for translation.  

6. **Custom Training Enhancements**  
   - **Custom Learning Rate Schedule** with warm-up.  
   - **Masked Loss & Accuracy** functions to handle padded tokens.  

7. **Training & Evaluation**  
   - Compiled the model with custom loss & metrics.  
   - Trained for 20 epochs on prepared datasets.  
   - Visualized loss & accuracy curves with Matplotlib.  

8. **Model Testing**  
   - Implemented a `translate()` function to generate French translations.  
   - Evaluated on sample test cases and compared with reference translations.  

### 🚀
