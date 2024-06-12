# Get Your Own Local AI Coding Copilot with LLAMA3

In this tutorial I'll show you how to set up your own local LLAMA3 copilot using CodeGPT and Ollama in Visual Studio Code. We'll install and configure the tools together.

If you prefer learning through a visual approach or want to gain additional insight into this topic, be sure to check out my YouTube video on this subject!

[![llama-copilot](/ollama/ollama-copilot/llama-copilot.png)](https://youtu.be/oGzJhKQfsGs)

## Quick Links

* Ollama
	* [Ollama website](https://ollama.com/)
	* [Ollama Models](https://ollama.com/library)
    * [How to install Ollama locally](/ollama/install-ollama/README.md)
* [Microsoft Visual Studio Code](https://code.visualstudio.com/)
* CodeGPT
    * [CodeGPT Website](https://codegpt.co/)
    * [CodeGPT Extension for VSCode](https://marketplace.visualstudio.com/items?itemName=DanielSanMedium.dscodegpt)

## Setup

To get started, you'll need:

* [**Ollama**](https://ollama.com/): an open-source tool for running large language models locally
* [**Microsoft Visual Studio Code (VSCode)**](https://code.visualstudio.com/): The editor of choice for this project, but any other editor can be used.
	+ Free and easy to install.
* [**CodeGPT Extension for VSCode**](https://marketplace.visualstudio.com/items?itemName=DanielSanMedium.dscodegpt)
    + Freemium and easy to install

## Setting Up CodeGPT

The setup process is very simple, consisting of just two steps.

### Step 1: Install CodeGPT Extension
Open Visual Studio Code and access the Extensions panel by clicking on the Extensions icon in the left-hand sidebar. Search for "CodeGPT" in the Extensions Marketplace and click the "Install" button to add it to your VS Code setup.

### Step 2: Configure CodeGPT with Ollama
From the Extensions panel, click on the CodeGPT icon, then expand the Provider selector and choose Ollama. In the Model selector, type the name of the model you want to use (e.g., Llama3:latest). Ensure that the model is downloaded into Ollama by running the command Ollama-list in any terminal.


**Example Use Cases**

* Generate code: Ask CodeGPT to generate code for you, such as a calculator app in Python.
* Get insight into code: Select the portion of the code you'd like explained and ask CodeGPT to break it down for you.
* Refactor code: Ask CodeGPT to refactor an if-else statement in your code.
