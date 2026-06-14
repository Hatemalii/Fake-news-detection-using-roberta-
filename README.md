# Fake News Detection Using RoBERTa

A transformer-based fake news detection system built by fine-tuning RoBERTa
on a combined dataset of WELFake and LIAR to classify news articles 
as real or fake.

## Project Goal
- Fine-tune a transformer model on a real-world misinformation dataset
- Handle dataset merging and label normalization across two different sources
- Evaluate model robustness across different news writing styles and sources

## Model
- Base model: `roberta-base`
- Task: Binary text classification (Real / Fake)
- Framework: Hugging Face Transformers

## Dataset
Combined two public datasets:
- **WELFake** — large-scale fake news dataset with 72,000+ articles
- **LIAR** — benchmark dataset with 12,800+ human-labeled short statements

Labels were normalized and merged to create a unified binary classification dataset.

## Results
| Metric | Score |
|--------|-------|
| Accuracy | 92% |
| F1 Score | 88% |
| Precision | 87% |
| Recall | 84% |

