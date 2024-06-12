# How to Use GGUF Files from Huggingface in Ollama

In this tutorial I'll demonstrate how to import any large language model from Huggingface and run it locally on your machine using Ollama, specifically focusing on GGUF files. As an example, I'll use the CapybaraHermes model from "TheBloke". The process is straightforward, and I'll guide you through each step in a clear and concise manner, making it easy for anyone to follow along.

If you prefer learning through a visual approach or want to gain additional insight into this topic, be sure to check out my YouTube video on this subject!

[![ollama-on-colab](/ollama/import-quantized-models-to-ollama/gguf-files-ollama-thumbnail.png)](https://youtu.be/vs1u9z2U4ZA)

## Quick Links

* Ollama
	* [Ollama website](https://ollama.com/)
	* [Installation Guide](/ollama/install-ollama/README.md)
	* [Ollama Documentation for Modelfiles](https://github.com/ollama/ollama/blob/main/docs/modelfile.md)
    * [Ollama Documentation for Importing Models](https://github.com/ollama/ollama/blob/main/docs/import.md)
    * [Mistral Model in Ollama Library](https://ollama.com/library/mistral)
* [Microsoft Visual Studio Code](https://code.visualstudio.com/)
* Hugging Face
    * [Hugging Face Website](https://huggingface.co)
    * [Capybara-Hermes Model](https://huggingface.co/TheBloke/CapybaraHermes-2.5-Mistral-7B-GGUF) from TheBloke

## Setup

Here's what I'll be using:

* [**Ollama**](https://ollama.com/): framework for running large language models locally
	+ Open-source and easy to set up
	+ [Link](/ollama/install-ollama/README.md) for installation process
* [**Microsoft Visual Studio Code (VSCode)**](https://code.visualstudio.com/): The editor of choice for this project, but any other editor can be used.
	+ Free and easy to install.
* [**An account with Hugging Face**](https://huggingface.co) for downloading quantized models (GGUF file)
    + Free and easy to sign up

## What are Quantized Models?

Quantized models are smaller versions of large language models that have been "shrunk" using a technique called quantization.

**How does Quantization work?**
It's like compressing a file into a zip archive. The goal is to reduce the size of the model so it can run efficiently on devices with limited resources, such as laptops or mobile phones.

**Trade-off between Precision and Accuracy:**
While quantization may lead to a trade-off between precision and accuracy, the impact is often not significant for everyday use cases. The quantized model can still perform remarkably well compared to its full-sized version.

In summary, quantized models are smaller versions of large language models that have been compressed using the quantization technique, allowing them to run efficiently on devices with limited resources.

## Finding Quantized Models in GGUF Format

### Step 1: Navigate to Huggingface MODELS Section
Head over to the Huggingface MODELS section and look for the tag list on the left side of the page.

### Step 2: Filter by GGUF Tag
Under LIBRARY, find the GGUF tag and click on it to narrow down your search results to only include models with a GGUF file.

#### Choosing the Right File

I'll be importing a model called [CapyBaraHermes 2.5 Mistral 7B - GGUF](https://huggingface.co/TheBloke/CapybaraHermes-2.5-Mistral-7B-GGUF) from TheBloke.

TheBloke provides a detailed overview of the available files and their implications.

Some files are more compressed, which means they may not be as accurate in their performance. Others are less compressed and therefore offer better accuracy.
It's up to you to decide what you need.

I'll be choosing the Q4 K.M version, which strikes a good balance between compression and quality.

To access the file, simply click on the link that leads to it and then press the download button.

## Importing a Quantized Model

1. [**Create a Modelfile**](#step-1---creating-a-modelfile):
    * Outline the specific guidelines for how your customized model should behave.
2. [**Generate the Actual Custom Model**](#step-2---generate-a-custom-model-from-modelfile):
    * Take the modelfile and generate the actual custom model.

### Step 1 - Creating a Modelfile

Either create a new modelfile from scratch and populate it manually - or copy the modelfile of the quantized model base model (Mistral 7b) for more efficiency
The command is:
``` markdown
ollama show <source-model-name> --modelfile > <target-modelfile-name>
```
Example:
``` markdown
ollama show mistral --modelfile > capyhermes-modelfile
```

### Step 2 - Generate a Custom Model from Modelfile
Create a custom model from the modelfile. 
The command is: 
``` markdown
ollama create <target-model-name> -f <target-modelfile-name>
```
For the Yoda-Example:
``` markdown
ollama create capyhermes -f capyhermes-modelfile
```
As a result, a new model called `capyhermes` will be created

## Improving your Imported Model
If you're not happy with the performance of your imported, or you want to change it, its 2 easy steps:
1. Remove your custom model using the instruction `ollama rm <custom-model-name>`
2. Change the instructions in the model file
3. Generate a custom model from the changed model file [(step 2)](#step-2---generate-a-custom-model-from-modelfile).

For example, please see [this tutorial](/ollama/customize-models/README.md) on creation custom models.