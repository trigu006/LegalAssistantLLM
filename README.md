# LegalAssistantLLM
This RAG model is a proof of concept that helps to answer questions on the contracts in its database, ideal for small-to-medium-sized legal practices.

## Environment setup
To create the virtual environment, please enter the command below in the "LegalAssistantLLM" directory. This will also download all the libraries in the "environment.yml" file.

```
conda env create -f environment.yml
```

You can then activate your environment via the command below. "LegalLLMEnv" is the name of the virtual environment and can be found as the "name" variable inside the "environment.yml" file.

```
conda activate LegalLLMEnv
```

## Background information

### Supported models

There are two models that are curently supported.
1. OpenAI (API calls) → **requires OpenAI API key in the .env file**
2. Ollama (locally installed [i.e., in your own computer] LLM)

### Contract or file uploads
To upload the documents that you would like to include in your RAG model, you can use the "Contracts" folder or create your own.

If you decide to create your own folder, please ensure that you pass the directory in the line below of the "Jupyter - Walkthrough" file.

```
documents = createPDFDocumentsFromDirectory('[Your directory goes here.]')
```
