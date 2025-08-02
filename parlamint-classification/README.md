# Ideology and Power Identification in Parliamentary Debates

This project demonstrates a machine learning pipeline for text classification using transformer models to identify ideology and power dynamics in parliamentary debates. It utilises Italian Orientation and Power data. The key steps are:

## Steps

1. **Data Preparation**  
   - The dataset is loaded, preprocessed, and split into training and testing sets.  
   - Two text columns (original and English-translated) are prepared for evaluation.

2. **Tokenization**  
   - Text is tokenized using a pre-trained tokenizer to convert it into a format suitable for transformer-based models.

3. **Fine-Tuning**  
   - A pre-trained transformer model (`FacebookAI/xlm-roberta-base`) is fine-tuned on labeled data to perform sequence classification.  

4. **Inference**  
   - Zero-shot classification using a pre-trained model (`facebook/bart-large-mnli`) is performed on both English-translated and original text without task-specific fine-tuning.

5. **Evaluation**  
   - The models are evaluated using metrics like accuracy, precision, recall, and f1-scores.  
   - Comparative analysis highlights the strengths and limitations of each approach.

6. **Results**  
   - Fine-tuned models achieve higher accuracy and balanced performance across classes.  
   - Zero-shot models are useful as a baseline but exhibit biases and perform better on English-translated text.

## Key Insights

- Fine-tuning improves task-specific performance significantly.  
- Zero-shot models can be a quick alternative when fine-tuning is not feasible but are language-dependent and less effective on non-English data.

This project demonstrates the benefits of fine-tuning for precise classification while offering zero-shot models as a baseline for flexible inference.
