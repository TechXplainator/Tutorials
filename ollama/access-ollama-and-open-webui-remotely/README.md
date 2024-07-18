
# Access Open WebUI from Your Phone or Anywhere

In this tutorial, we will show you how to run a large language model privately and for free on your local machine, giving you the power to access it from anywhere in the world. We'll be using Ollama, Docker, Open WebUI, and Ngrok.

If you prefer learning through a visual approach or want to gain additional insight into this topic, be sure to check out my YouTube video on this subject!

[![ollama-on-the-go](/ollama/access-ollama-and-open-webui-remotely/ollama-on-the-go-thumbnail.png)](https://youtu.be/Gys4_I5fvTs)

## Quick Links

* Ollama
	* [Ollama website](https://ollama.com/)
	* [Ollama Models](https://ollama.com/library)
    * [How to install Ollama locally](/ollama/install-ollama/README.md)
* Open WebUI
	* [GitHub Page](https://github.com/open-webui/open-webui)
	* [Installation Commands](https://github.com/open-webui/open-webui?tab=readme-ov-file#installation-with-default-configuration)
    * [How to install Open WebUI](/ollama/open-webui/README.md)
    * Localhost URL for OpenWebUI: [http://localhost:3000](http://localhost:3000)
* Docker 
    * [Docker Website](https://www.docker.com/products/docker-desktop/)
* Ngrok
    * [Ngrok Website](https://ngrok.com/)

## What You'll Need

* **Ollama**: A framework that lets you run large language models locally on your machine.
* **Docker**: Software that enables applications to run within containers, allowing them to function regardless of your operating system.
* **Open WebUI**: An open-source tool making it simpler to interact with large language models.
* **Ngrok**: A software that gives your local web applications a public URL.

## Installation Steps

### Step 1: Install Ollama

1. Download Ollama from the official [Ollama website](https://ollama.com/).
2. Verify that Ollama has been successfully installed by looking for the Lama Icon in the menu bar.

If you need more detailed install-instructions, checkout the page on [how to install Ollama locally](/ollama/install-ollama/README.md).

### Step 2: Install Docker

1. Visit the [Docker Website](https://www.docker.com/products/docker-desktop/) and download the application for your operating system.
2. Complete the setup process, accepting the user agreement and using the recommended settings.
3. Verify that Docker is running by noticing the new Docker icon on your menu bar.

### Step 3: Install Open WebUI

1. Head over to the Open WebUI repository on GitHub.
2. Copy the installation command from the README file and paste it into the Terminal.
3. Confirm that Open WebUI has been successfully installed by navigating to `localhost:3000` in your web browser.

For more detailled install-instruction, check out the page on [how to install Open WebUI](/ollama/open-webui/README.md)

### Step 4: Install Ngrok

1. Sign up for a free account on [ngrok.com](https://ngrok.com/).
2. Follow the installation instructions for your operating system. For Mac OS, enter the command `brew install ngrok/ngrok/ngrok` into your terminal app to trigger the installation
3. Authenticate your local machine using the authentication code provided during sign-up. The command is `ngrok config add-authtoken <YOUR AUTHENTICATION CODE FROM NGROK>`

## Access Ollama from Your Phone via Open WebUI

1. Use Ngrok to create a public URL that allows you to access Open WebUI remotely. You will find the command to do that on their "Setup & Installation" page. However, you need to adapt the port to the port of the app you're running. For example, Open WebUI is running on `localhost:3000`, so you must change the port in the Ngrok command to `3000`. Specifically:
    * The command given on the Ngrok page is `ngrok http http://localhost:8080`
    * To forward the Open WebUI app, you must change this command to `ngrok http http://localhost:3000`
2. Copy the forwarding URL that Ngrok gives you in the terminl
3. Enter the forwarding URL into a new browser window on your phone or any device with internet access.
4. Log in with your user credentials and start interacting with the large language model using Open WebUI.

That's it! With these steps, you should be able to access your own large language models privately and for free from anywhere in the world.