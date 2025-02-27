# To AI, or Not to AI A Deep Learning Approach to Detect AI Generated Text

## Description

This project addresses the challenge of distinguishing between AI-generated text and human-written content, amidst concerns about academic integrity and misinformation raised by the rise of Generative AI and Large Language Models such as ChatGPT and GPT-4. It entails developing and optimizing neural networks, with a focus on fine-tuning three transformer models from Hugging Face, all of which are RoBERTa-based, to accurately identify AI-generated text. This initiative is critical in combating AI's potential for spreading false information and ensuring the credibility of online content. The project promotes responsible AI use and advances detection methods in the digital realm.

## Usage

To run the main notebook, open `main.ipynb` in a Jupyter notebook environment.
By running the following command:

```bash
jupyter notebook main.ipynb
```

You can also directly access our fine-tuned and ensembled model on hugging face, and try it:

[`Huggin Face Space 🤗`](https://huggingface.co/spaces/rusen/gpt_detector)


## Installation

To install the project's dependencies, run the following command:

```bash
pip install -r requirements.txt
```

The base models should download automatically when running the main notebook. However, if you want to download them manually, you can click on the model name and download the following models:

- [`roberta-base`](https://huggingface.co/roberta-base-openai-detector)
- [`ChatGPT-Detector`](https://huggingface.co/Hello-SimpleAI/chatgpt-detector-roberta)
- [`ChatGPT-Detector-LLI`](https://huggingface.co/Nintw923/chatgpt-detector-lli-hc3)

Or you can download them on the following google drive link:

- [Google Drive Link](https://drive.google.com/drive/folders/1AxTw-65OnvyHT71_XQSLDNeeadI7yXij?usp=sharing)

Additionally, link to the pre-data we used:

[Pre-Data](https://github.com/dukeraphaelng/synth_detectives)

## Data

The data used in this project is located in the `Data/` directory. Here's a brief description of each file:

- `ai.csv`: This file contains data generated by an AI (GPT-3.5).
- `data-prepare.ipynb`: This file is a Jupyter notebook used for data preparation.
- `final_data.csv`: This file contains the final processed data.
- `human.csv`: This file contains data generated by humans.
- `pre-made.csv`: This file contains pre-made data from the internet.
- `youtube_comments.csv`: This file contains data extracted from YouTube comments.
- `The Da Vinci Code.pdf` and `The Diary of a Young Girl.pdf`: These are examples of what we have used as PDF sources.
  
## Scripts

The `Scripts/` directory contains utility scripts used in this project:

- `utils.py`: This file contains utility functions for handling transformer models. It includes functions to download, load, and save transformer models and their tokenizers (`get_model`), make predictions on a batch of sentences (`model_predict`), and evaluate model performance by computing accuracy, recall, precision, and F1-score (`eval_model`).

## Contributing

This project is not open to contributions at this time.
This project is created by [Ruşen Birben](https://github.com/rusenbb) and [Burak Ercan](https://github.com/BurakErcn).
