# Creating AI Agents with Ollama

In this tutorial, we're going to build AI agents on Google Colab with the help of LLaMA3 powered by Ollama. 

With these powerful tools, you can automate tasks that would normally take hours or days, such as preparing for meetings, generating customized trip plans, or writing blogs and social media posts. 

The good news is that this process is entirely free!

If you prefer learning through a visual approach or want to gain additional insight into this topic, be sure to check out my YouTube video on this subject!

[![ollama-agents](

## Quick Links

* Jupyter Notebooks
* Ngrok
	* [Ngrok website](https://ngrok.com/)
	* [Getting free static domains in Ngrok](https://ngrok.com/blog-post/free-static-domains-ngrok-users)
* Ollama
	* [Ollama website](https://ollama.com/)
	* [How to install Ollama locally](/ollama/install-ollama/README.md)
    * [How to run Ollama on Google Colab](/ollama/ollama-on-colab/README.md)
* Google Colab
	* [Google Colab website](https://colab.research.google.com/)

## Setup

Here's what I'll be using:

* [Ollama](https://ollama.com/): framework for running large language models locally
	+ Open-source and easy to set up
	+ [Link]((/ollama/install-ollama/README.md)) for installation process
* [Google Colab](https://colab.research.google.com/): cloud-based platform for Python code and Jupyter notebooks
	+ Free account required, assumes you already have one
	+ Consider upgrading to [Colab Pro](https://colab.research.google.com/signup/pricing) for faster LLMs
* [Ngrok](https://ngrok.com/): gives local web applications a public URL
	+ Sign up for free account in description



## Setup Steps

1. [Expose local Ollama to public URL provided by Ngrok]()
2. [Open a pre-prepared Jupyter Notebook on Colab, logged in with Google account.]()
3. [Execute the code in Jupyter Notebook]()



### Step 1 - Expose local Ollama to public URL provided by Ngrok

When it comes to exposing Llama3 to Google Colab with Ngrok, you have two viable options. One approach is to install Ngrok on your machine and map your URL - a very straightforward process! Alternatively, you can run Llama3 directly on Colab using a Ngrok URL, without any installation to your local machine.

#### Option 1 - Install Ngrok and Expose your local URL

On your local machine:
 * Install ngrok: https://ngrok.com/download
 * Open a terminal and run: `ngrok http http://localhost:11434`
 * Copy the forwarding URL (it will be something like https://1234-your-ngrok-url.ngrok.io)

#### Option 2 - Run llama3 on Google Colab using Ngrok

I created a comprehensive tutorial that utilizes a static URL from Ngrok, allowing me to reuse it multiple times. You can find the tutorial here: [Running Ollama on Google Colab](/ollama/ollama-on-colab/README.md).


### Step 2: Open Prepared Jupyter Notebook

* Open this [Jupyter notebook]() in Google Colab
* Ensure logged in with Google account first
* Navigate to "Secrets" section within Colab
* Add new secret and name it `OLLAMA_BASE_URL`. Now add the Ngrok URL from [step 1](#step-1---expose-local-ollama-to-public-url-provided-by-ngrok) as a value. 
* Add new secret called `OLLAMA_MODEL` and insert the name of the model you want to use via Ollama. In our case, it's `llama3`.
* Don't forget to enable notebook access for both values!


### Step 3: Execute Jupyter Notebook

* Run all cells in the notebook
* You should see a printed output of your crew's work.