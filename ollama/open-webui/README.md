# Installing Open WebUI for Ollama

This tutorial will guide you through setting up Open WebUI for Ollama, an open source software which allows you to interact with LLMs through a friendly web interface, eliminating the need for CLI commands.

If you prefer learning through a visual approach or want to gain additional insight into this topic, be sure to check out my YouTube video on this subject!

[![ollama-on-colab](/ollama/open-webui/open-webui-thumnail.png)](https://youtu.be/0DFJc-oIRQ8)

## Quick Links

* Ollama
	* [Ollama website](https://ollama.com/)
	* [Ollama Models](https://ollama.com/library)
    * [How to install Ollama locally](/ollama/install-ollama/README.md)
* Open WebUI
	* [GitHub Page](https://github.com/open-webui/open-webui)
	* [Installation Commands](https://github.com/open-webui/open-webui?tab=readme-ov-file#installation-with-default-configuration)
* [Docker Website](https://www.docker.com/products/docker-desktop/)
* Localhost URL for OpenWebUI: [http://localhost:3000](http://localhost:3000)

## Setup

To get started, you'll need:

* [**Ollama**](https://ollama.com/): an open-source tool for running large language models locally
* [**Docker**](https://www.docker.com/products/docker-desktop/): software that enables applications to run within containers
* [**Open Web UI**](https://github.com/open-webui/open-webui): a tool making it simpler to interact with LLMs

## Installation Steps


### Step 1: Install Ollama & Download Models
* Install Ollama. See prior [documentation](/ollama/install-ollama/README.md) for details.
* Proceed to Step 2

### Step 2: Install Docker
* Visit the [Docker website](https://www.docker.com/products/docker-desktop/) and download the application for your operating system (e.g., Mac)
* Follow installation prompts, accepting user agreement and using recommended settings
* Verify installation by noticing the new Docker icon on your menu bar

### Step 3: Install Open WebUI in a Docker Container
* Go to the [Open WebUI repository on GitHub](https://github.com/open-webui/open-webui?tab=readme-ov-file#installation-with-default-configuration)
* Copy the installation command for installing Open WebUI in a Docker container, including dependencies. Here it is once more for your information:
```
docker run -d -p 3000:8080 --add-host=host.docker.internal:host-gateway -v open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:main
```
* Paste the command into any Terminal application and run it
* Verify installation by opening the Docker app and checking that Open WebUI is installed

### Step 4: Open WebUI Sign-In
* Navigate to the Open WebUI URL [http://localhost:3000](http://localhost:3000)
* Sign up for an admin user account, providing full name, email address, and password
* Keep in mind that this information will not be validated or stored externally

## Adding a new model

1. Navigate to the model selection in Open WebUI (Top of the page) and search for the desired model (e.g., "Mistral").
2. Type the model name into the search bar and select the option to "pull mistral from ollama.com".
3. The model will be downloaded directly from Ollama.com to your local machine via Ollama.
4. Wait for the download to complete, then check the dropdown menu for the newly added model.

> Your user must be an administrator for "pull model" to appear!

## Ending and Restarting Open Web UI

1. Close the browser window to exit Open WebUI.
2. To stop using Open WebUI, open the Docker app, locate the container hosting Open WebUI, and click "Stop".
3. If you want to access Open WebUI again, restart the Docker container by clicking the play button.