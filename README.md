<a href="https://colab.research.google.com/github/LeonardSEO/Data-Preparation-and-Generation-for-LLM-Training/blob/main/PDF_to_LLM_Dataset_Creator.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> 

<a href="https://www.linkedin.com/in/leonard-van-hemert/" target="_parent">
  <img src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA3MiA3MiI+PHBhdGggZD0iTTY2LjE0IDBINFg4NkE1Ljg2IDUuODYgMCAwIDAgMCA1Ljg2djYwLjI4QTUuODYgNS44NiAwIDAgMCA1Ljg2IDcyaDYwLjI4QTUuODYgNS44NiAwIDAgMCA3MiA2Ni4xNFY1Ljg2QTVuODYgNS44NiAwIDAgMCA2Ni4xNCAwei0xLjk3IDEyLjk1YTYuMzg2LjM4IDAgMSAxLTYxMyAwIDAgMSA0LjY3MyAwLTYgMzAuNTNzNi4zNnQwIDB6TTM2IDEuNzloLTdWMjY4MkgzdWE0d3NlLWwiIGZpbGw9IiNFQ0UgU29keSIlIC8+PC9zdmc+" alt="LinkedIn Profile"/>
</a>


# PDF-to-LLM Dataset Creator

This repository provides a Google Colab notebook designed to create a dataset for training a language model using text extracted from a PDF. The notebook guides you through the process of setting up the necessary environment, extracting text from a PDF, generating examples based on a user-provided prompt, and formatting the data into a JSONL file suitable for machine learning tasks.

## Features

- **Extract Text from PDF**: Automatically download and process a PDF from a provided URL.
- **Generate Dataset Examples**: Utilize the OpenAI API to generate diverse and high-quality examples based on a given prompt.
- **Prepare JSONL Dataset**: Format and clean the generated examples into training and testing datasets in JSONL format.
- **Downloadable Output**: Easily download the resulting dataset files for use in training language models.

## Parameters

1. **prompt**: A high-level description of the type of model to be trained.
2. **temperature**: A value between 0 and 1 controlling the randomness of the generated examples.
3. **number_of_examples**: The total number of examples to generate.
4. **pdf_url**: The URL where the PDF to extract information from can be accessed online.

### Example Parameters

```python
prompt = "A model that takes in a puzzle-like reasoning-heavy question in English, and responds with a well-reasoned, step-by-step thought out response in Spanish."
temperature = 0.4
number_of_examples = 100
pdf_url = "https://example.com/path/to/your/pdf.pdf"
