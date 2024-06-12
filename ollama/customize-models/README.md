# How to Build a Custom Local Version of LLAMA3

This tutorial will guide you through customizing any large language model and run it locally on your machine using Ollama. As a demonstration, I'll use LLAMA3 to create a custom version that behaves like Yoda from the Star Wars movies. The process is straightforward, and I'll walk you through each step, making it easy for anyone to follow along.

If you prefer learning through a visual approach or want to gain additional insight into this topic, be sure to check out my YouTube video on this subject!

[![ollama-on-colab](/ollama/customize-models/customize-ollama-models-thumbnail.png)](https://youtu.be/gyX-N-ppU3E)

## Quick Links

* Ollama
	* [Ollama website](https://ollama.com/)
	* [Installation Guide](/ollama/install-ollama/README.md)
	* [Ollama Documentation for Modelfiles](https://github.com/ollama/ollama/blob/main/docs/modelfile.md)
* Open WebUI
	* [GitHub Page](https://github.com/open-webui/open-webui?tab=readme-ov-file#open-webui-formerly-ollama-webui-)
	* [Installation Guide](/ollama/open-webui/README.md)
* [Microsoft Visual Studio Code](https://code.visualstudio.com/)	

## Setup

Here's what I'll be using:

* [**Ollama**](https://ollama.com/): framework for running large language models locally
	+ Open-source and easy to set up
	+ [Link](/ollama/install-ollama/README.md) for installation process
* [**Microsoft Visual Studio Code (VSCode)**](https://code.visualstudio.com/): The editor of choice for this project, but any other editor can be used.
	+ Free and easy to install.

## Creating a Customized Model

1. [**Create a Modelfile**](#step-1---creating-a-modelfile):
    * Outline the specific guidelines for how your customized model should behave.
2. [**Generate the Actual Custom Model**](#step-2---generate-a-custom-model-from-modelfile):
    * Take the modelfile and generate the actual custom model.

### Step 1 - Creating a Modelfile
1. Copy the modelfile of LLAMA3 for more efficiency
The command is:
``` markdown
ollama show <source-model-name> --modelfile > <target-modelfile-name>
```
Example:
``` markdown
ollama show llama3 --modelfile > yoda-modelfile
```
2. Change the newly created modelfile `yoda-modelfile` to add your custom instructions. For example, like in this [example](/ollama/customize-models/yoda-modelfile) and save your file

### Step 2 - Generate a Custom Model from Modelfile
Create a custom model from the modelfile. 
The command is: 
``` markdown
ollama create <target-model-name> -f <target-modelfile-name>
```
For the Yoda-Example:
``` markdown
ollama create yoda-llama -f yoda-modelfile
```
As a result, a new model called `yoda-llama` will be created

## Changing the Custom Instructions
If you're not happy with the performance of your custom model, or you want to change it, its 2 easy steps:
1. Remove your custom model using the instruction `ollama rm <custom-model-name>`
2. Change the instructions in the model file
3. Generate a custom model from the changed model file [(step 2)](#step-2---generate-a-custom-model-from-modelfile)



