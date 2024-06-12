# Getting Started with Ollama

This tutorial will guide you through setting up Ollama locally on your machine.

If you prefer learning through a visual approach or want to gain additional insight into this topic, be sure to check out my YouTube video on this subject!

#<iframe width="560" height="315" src="https://youtu.be/76uPAMvsTyM" frameborder="0" allowfullscreen></iframe>

## Quick Links

* Ollama
	* [Ollama website](https://ollama.com/)
	* [Ollama Models](https://ollama.com/library)

## Ollama Hardware Requirements

* Compatibility with:
	+ MacOS running on Apple Silicon
	+ Linux distributions (Debian, Ubuntu)
	+ Microsoft Windows
* Recommended hardware for best performance:
	+ On Linux and Windows systems: modern GPU (Nvidia or AMD)
	+ On Mac systems: M1, M2, or M3 chips
* Note that each model may have unique requirements beyond these basic specifications


## Reasons for Running AI Locally

1. **Data Control**: Run your own local LLM to maintain full control over data and avoid sending sensitive information to external servers.

2. **Cost-Effectiveness**: Paying up to $20/month for GPT-4 or other commercial models might not be feasible for everyone. Open-source AI models offer excellent features without breaking the bank.

3. **Convenience**: With local AI, you can access your digital assistant regardless of your internet connection. Perfect for situations where Wi-Fi is unreliable or non-existent (e.g., on a flight or in a remote area).

4. **Model Customization**: Ollama offers various models for download, including specialized ones for mathematical problem-solving, coding, and unrestricted variants. This flexibility allows you to tailor your AI experience to your specific needs.

## Installing Ollama:

1. Go to Ollama's official website and select "download" for your specific operating system.

2. Follow the download and installation process, which is similar to installing any software from the web and consistent across different operating systems.

## Running Ollama on MAC

* Ollama operates using a command line setup, which may require some adjustment for those not familiar with it.
* On Macs, the terminal app can be accessed via Spotlight Search:
	+ Press Command + Spacebar to open Spotlight Search
	+ Type 'Terminal' into the search bar and hit Enter

### Ollama Commands

```markdown
Usage:
  ollama [flags]
  ollama [command]

Available Commands:
  serve       Start ollama
  create      Create a model from a Modelfile
  show        Show information for a model
  run         Run a model
  pull        Pull a model from a registry
  push        Push a model to a registry
  list        List models
  ps          List running models
  cp          Copy a model
  rm          Remove a model
  help        Help about any command

Flags:
  -h, --help      help for ollama
  -v, --version   Show version information

Use "ollama [command] --help" for more information about a command.
 ```

## Choosing and Downloading a Model

* Ollama supports various [models](https://ollama.com/library), including Meta's LLaMA, Google's Gemma, Mistral, and others like uncensored LLaMA2 or LAVA (which handles images and media).
* Each model has its own page on the site, providing details on:
	+ What it's good at
	+ File size
	+ Hardware requirements
* Choosing a model involves considering the number of parameters (inner workings that help the model understand data):
	+ More parameters usually mean a more powerful model, but they require more GPU resources.
	+ Models with more parameters tend to perform better, but be mindful of your GPU's limits.
* General guidelines for GPU requirements:
	+ 7B models: at least 8 GB RAM
	+ 13B models: at least 16 GB RAM
	+ 33B models: at least 32 GB RAM
* Every model takes up space on your machine, and you can see the required space in the dropdown menu.
* Once you've chosen a version, copy the command and paste it into your terminal to download and set up the model:
	+ For example, grabbing the [8B LLaMA3 version](https://ollama.com/library/llama3) - the command to run the model would be `ollama run llama3`
    ![find-run-command](/ollama/install-ollama/find-run-command-for-model.png) 

## Interacting with a Model

* Communicate with your installed model by typing prompts or questions.
* Use the command `/?` to access a menu of available commands, starting with a slash. Otherwise, the model will interpret everything as a prompt.
* Exit interaction mode by using the command `/bye`
