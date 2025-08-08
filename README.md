# Sentiment Analysis Toolkit – TextBlob & BERT

This repository contains two complete projects that demonstrate how to perform **sentiment analysis** on text using two very different approaches:  
1. **TextBlob** – a lightweight, rule-based method.  
2. **BERT** – a deep learning transformer model.

Both notebooks are designed to be educational, self-contained, and easy to run. They cover the process from loading text to producing interpretable sentiment scores or classifications.

---

## 1. Purpose of This Repository

Sentiment analysis is the process of determining whether a piece of text expresses a **positive**, **negative**, or **neutral** sentiment. It is widely used in:

- Product review analysis
- Stock analysis
- Social media monitoring  
- Customer feedback interpretation  
- Market research  

---

## 2. Project Descriptions

### **Sentiment Analysis with TextBlob**

- **Approach**: TextBlob is a **Python library for processing textual data** that builds on top of NLTK (Natural Language Toolkit) and Pattern.  
For sentiment analysis, it uses a **lexicon-based approach**, where each word has an associated polarity score (ranging from –1 for negative to +1 for positive) and subjectivity score (0 for objective to 1 for subjective).  
The sentiment of a sentence is calculated by combining these word-level scores according to simple rules.  

- **Advantages**:  
  - Requires no training data.  
  - Very fast, even on limited hardware.  
  - Easy to implement in just a few lines of code.  
- **Limitations**:  
  - Does not handle sarcasm or nuanced sentiment well.  
  - Struggles with domain-specific vocabulary.  

---

### **Sentiment Analysis with BERT**

- **Approach**: Uses a pre-trained deep learning model (**Bidirectional Encoder Representations from Transformers**) fine-tuned for sentiment classification.
Unlike older models that read text left-to-right or right-to-left, BERT reads **both directions simultaneously** (*bidirectional*), enabling it to understand the meaning of words based on their surrounding context.  
For sentiment analysis, BERT is often **fine-tuned** on labeled datasets so it can classify text as *positive*, *negative*, or *neutral* with high accuracy.  
- **Advantages**:  
  - Captures complex patterns in language.  
  - Understands context, negations, and subtleties better than lexicon-based methods.  
  - Adaptable to different languages and domains with fine-tuning.  
- **Limitations**:  
  - Requires more processing power (**GPU recommended**).  
  - Slightly slower to run than rule-based methods.


By exploring both approaches, you will understand the trade-offs between speed and accuracy, simplicity and complexity, and rule-based vs. machine learning approaches.

---

## 3. Repository Structure

```plaintext
Stock-Sentiment-Analysis/
│
├── Sentiment-Analysis-TextBlob.ipynb    # Jupyter notebook using TextBlob
├── Sentiment-Analysis-BERT.ipynb        # Jupyter notebook using BERT
└── README.md                            # Project documentation

