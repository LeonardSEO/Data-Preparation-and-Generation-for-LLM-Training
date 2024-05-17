<a href="https://colab.research.google.com/github/LeonardSEO/Data-Preparation-and-Generation-for-LLM-Training/blob/main/PDF_to_LLM_Dataset_Creator.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> <a href="https://www.linkedin.com/in/leonard-van-hemert/" target="_parent"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" width="20" height="20"><path d="M100.28 448H7.4V149.5h92.88zm-46.14-340C24.43 108 0 83.54 0 53.57A53.58 53.58 0 0 1 54.14 0c30 0 54.22 24.43 54.22 54.14S84.17 108 54.22 108zm394.18 340h-92.68V302.4c0-34.68-.7-79.29-48.3-79.29-48.3 0-55.7 37.72-55.7 76.7v148.2H161.92V149.5h89v40.8h1.3c12.4-23.5 42.57-48.3 87.55-48.3 93.63 0 110.77 61.6 110.77 141.78V448z"/></svg></a>



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
