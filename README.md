# Hindi Article Generator 📰

This project is a Hindi Article Generator, developed using natural language processing (NLP) techniques to create contextually relevant and coherent articles in Hindi. The model was trained on a custom dataset collected via web scraping. The model has been fine-tuned on a dataset of Hindi news headlines and articles to generate high-quality, fluent articles for a variety of use cases such as news, blogs, and creative content.

## 🚀 Quick Start (Google Colab)

1. Open [Google Colab](https://colab.research.google.com/)
2. Upload the notebook: `File → Upload notebook → Select hindi_article_generator_colab.ipynb`
3. Enable GPU: `Runtime → Change runtime type → GPU (T4)`
4. Run all cells - you'll be prompted to upload the dataset CSV file
5. Generate Hindi articles from headlines!

## 📁 Dataset

The model is trained on a dataset that I created through web scraping from the BBC Hindi website. The dataset includes:
- **4,796 Hindi news articles**
- Multiple categories (भारत, विश्व, खेल, etc.)
- Headlines with corresponding full articles

## 🛠️ Tech Stack

- **Model**: Llama-3 8B (4-bit quantized)
- **Fine-tuning**: LoRA adapters via Unsloth
- **Framework**: PyTorch, Transformers, TRL
- **Platform**: Google Colab (free GPU)

## 📌 Features

* Generates fluent and contextually accurate Hindi articles from headlines
* Fine-tuned Llama-3 model optimized for Hindi language generation
* Efficient 4-bit quantization - runs on free Colab T4 GPU
* LoRA fine-tuning for memory-efficient training

## 🔄 Other Possible Tasks

This same dataset and approach can be used for:
1. Generating a headline for an article
2. Classification of an article into different categories
3. Classification of an article headline into different categories

## 📂 Files

| File | Description |
|------|-------------|
| `hindi_article_generator_colab.ipynb` | Main notebook (run on Google Colab) |
| `bbc_hindi_articles_with_categories_cleaned.csv` | Training dataset |
| `Inferences.md` | Sample model outputs |

## 📝 Usage Example

```python
headline = "भारतीय शेयर बाजार में तेजी"
category = "भारत"

# Model generates a complete Hindi article based on the headline!
```
