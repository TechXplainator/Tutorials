# Running Ollama on Google Colab

This tutorial will guide you through setting up Ollama in Google Colab using N-Grok. 

If you prefer learning through a visual approach or want to gain additional insight into this topic, be sure to check out my YouTube video on this subject!

[![ollama-on-colab](/ollama/ollama-on-colab/ollama-colab-thumbnail.png)](!!!!!!!!!!)

## Quick Links

* Jupyter Notebooks
	* [Run Ollama on Colab](/ollama/ollama-on-colab/run-ollama-on-colab.ipynb) from TechXplainator
	* [Run Ollama on Colab with models stored on Google Drive](/ollama/ollama-on-colab/run-ollama-on-colab-gdrive-storage.ipynb) from TechXplainator
	* [Original notebook](https://github.com/ollama/ollama/blob/5687f1a0cfa3d2408bfcb04f4342f657f6dada58/examples/jupyter-notebook/ollama.ipynb) from Ollama
* Ngrok
	* [N-Grok website](https://ngrok.com/)
	* [Getting free static domains in Ngrok](https://ngrok.com/blog-post/free-static-domains-ngrok-users)
* Ollama
	* [Ollama website](https://ollama.com/)
	* [How to install Ollama locally](/ollama/install-ollama/README.md)
* Google Colab
	* [Google Colab website](https://colab.research.google.com/)
	* [Colab price tiers](https://colab.research.google.com/signup/pricing)

## Setup

Here's what I'll be using:

* [Ollama](https://ollama.com/): framework for running large language models locally
	+ Open-source and easy to set up
	+ [Link]((/ollama/install-ollama/README.md)) for installation process
* [Google Colab](https://colab.research.google.com/): cloud-based platform for Python code and Jupyter notebooks
	+ Free account required, assumes you already have one
	+ Consider upgrading to [Colab Pro](https://colab.research.google.com/signup/pricing) for faster LLMs
* [N-Grok](https://ngrok.com/): gives local web applications a public URL
	+ Sign up for free account in description


## Downsides of running Ollama on Google Colab

* **Loss of privacy**. interactions with LLMs are no longer private as Google Colab and N-Grok can see every HTTP request
* **Cost associated with setup**
	+ Requires Colab Pro subscription for powerful GPU runtimes
	+ Ongoing monthly expense to factor into budget

## Setup Steps

1. [Log in to N-Grok and obtain authentication token and stable domain.](#step-1-get-authentication-token-and-stable-domain-from-n-grok)
2. [Open a pre-prepared Jupyter Notebook on Colab, logged in with Google account.](#step-2-open-prepared-jupyter-notebook)
3. [Copy and paste N-Grok authentication code into Colab notebook.](#step-3-maintain-auth-token-in-colab)
4. [Execute Jupyter Notebook, setting up Ollama on Colab and linking it to public stable N-Grok URL.](#step-4-execute-jupyter-notebook)
5. [Connect local Ollama to public N-Grok URL.](#step-5-connect-local-ollama-to-public-n-grok-url)
6. [Run Ollama.](#step-6-run-ollama)


### Step 1: Get Authentication Token and Stable Domain from N-Grok
* Access your N-Grok account
* Get your unique authentication token by clicking on "Your Auth-Token"
* Copy the token at the top of the page

Optional:
* Navigate to "Domains" section
* Create a static domain if you don't already have one

### Step 2: Open Prepared Jupyter Notebook

* Open this [Jupyter notebook](/ollama/ollama-on-colab/run-ollama-on-colab.ipynb) in Google Colab
* Ensure logged in with Google account first

### Step 3: Maintain Auth Token in Colab

* Navigate to "Secrets" section within Colab
* Add new secret and name it 'NGROK_AUTH_TOKEN'
* Paste authentication code from Ngrok into value field
* Enable notebook access
* Replace '<insert-your-statik-ngrok-domain-here>' in line 12 of last cell with the static domain you copied from Ngrok

> If you're NOT using a static Ngrok URL, uncomment line 11 and comment line 12 in the final cell of the notebook!


### Step 4: Execute Jupyter Notebook

* Run all cells in the notebook
* Output should be the following:

```markdown
"started tunnel" obj=tunnels name=command_line addr=http://localhost:11434 url=https://example.ngrok-free.app
```
> If you are using a static Ngrok URL, the example URL should correspond to the static Ngrok domain. If not, you will get a randomly generated URL from Ngrok.

### Step 5: Connect Local Ollama to Public N-Grok URL

* Copy generated URL from notebook's output
* Open command-line tool like Terminal app on Mac
* Configure local Ollama installation to communicate with instance hosted on Colab using the following command: "export Ollama_HOST=<paste_url_here>"
* Store stable URL for future reference if using a static URL

### Step 6: Run Ollama

* Start by running `Ollama List` and notice that model list is empty
* Download a model, such as Llama3, using the command `Ollama run llama3`
* Interact with Ollama locally and notice fast interaction due to leveraging Google's servers through Colab environment


## Ending and Restarting Ollama on Colab

* End Ollama by disconnecting and deleting runtime in Google Colab
* To restart Ollama:
	1. run the Jupyter notebook ([step 4](#step-4-execute-jupyter-notebook))
	2. export Ollama host variable ([step 5](#step-5-connect-local-ollama-to-public-n-grok-url))

## Alternative Method: Installing Ollama Models on Google Drive

* Install models directly on Google Drive using this alternative [Jupyter Notebook]((/ollama/ollama-on-colab/run-ollama-on-colab-gdrive-storage.ipynb))
* Note that running Ollama with models stored on Google Drive can result in slower performance and occasional connectivity issues with N-Grok

## Combining with Ollama WebUI

If using Ollama alongside with [Ollama WebUI](https://github.com/open-webui/open-webui), you'll need to do one additional step:

Install Open Web UI into a Docker container using the URL provided by N-Grok (stable URL required)

```markdown
docker run -d -p 4000:8080 -e OLLAMA_BASE_URL=<paste_url_here> -v open-webui:/app/backend/data --name ngrok-open-webui --restart always ghcr.io/open-webui/open-webui:main
```

This will create a docker container called `ngrok-open-webui`which lets Open WebUI run on http://localhost:4000/
