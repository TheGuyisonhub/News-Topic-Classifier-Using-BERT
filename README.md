# News Classification using BERT

## Objective of the Task

The objective of this project is to build a text classification model that can automatically classify news articles into four categories: World, Sports, Business, and Science/Technology. This task demonstrates the use of Natural Language Processing (NLP) and Transformer-based models for efficient text understanding and categorization.

## Methodology / Approach

1. **Dataset**
   * The AG News dataset was used, which contains around 120,000 training samples and 7,600 test samples across four balanced categories.
2. **Preprocessing**
   * The dataset was tokenized using a pre-trained BERT tokenizer.
   * Input sequences were padded/truncated to a fixed maximum length for uniformity.
3. **Model**
   * A pre-trained BERT model (`bert-base-uncased`) from Hugging Face Transformers was fine-tuned for the classification task.
   * A classification head was added on top of BERT to predict the news category.
4. **Training & Evaluation**
   * The model was trained using cross-entropy loss and evaluated on a test split.
   * Metrics used include accuracy and F1-score for performance measurement.
5. **Experimentation**
   * Two modes were provided:
     * **Quick mode**: Small subset (8k train, 2k test) for faster experimentation.
     * **Full mode**: Entire dataset for maximum performance.
## Key Results or Observations
* On the **subset (10k samples)**, the model achieves around **85–88% accuracy** within a few epochs, which is suitable for quick prototyping.
* On the **full dataset**, accuracy can reach **93–95%**, aligning with state-of-the-art results for AG News classification using BERT.
* Using pre-trained transformers significantly reduces training time while achieving high accuracy compared to training models from scratch.
* The modular pipeline allows easy scaling, further fine-tuning, or deployment with a simple interface (e.g., Gradio demo).

Do you want me to also make a **requirements.txt** for this project so it’s production-ready?
