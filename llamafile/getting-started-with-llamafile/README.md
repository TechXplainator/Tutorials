# Getting Started with Llamafile

This tutorial shows how to set up and run a large language model (LLM) using Llamafile. Llamafile is an open-source project that makes it easy for anyone to run large language models (LLMs) locally on their machine without requiring technical expertise. Just download and execute the file, and you're set! You'll learn how to download and install an LLM, change permissions, and run it in your terminal.

If you prefer learning through a visual approach or want to gain additional insight into this topic, be sure to check out my YouTube video on this subject!

[![get-started-llamafile-thumbnail](/llamafile/getting-started-with-llamafile/get-startet-with-llamafile-thumbnail.png)](https://youtu.be/IkzmOzy1maE)

## Quick Links

* Llamafile
	+ [Llamafile GitHub page](https://github.com/Mozilla-Ocho/llamafile?tab=readme-ov-file#llamafile)


## Setting Up and Running Llamafile Models

### Step 1: Download a Model
Head over to the [Llamafile GitHub page](https://github.com/Mozilla-Ocho/llamafile?tab=readme-ov-file#llamafile) and explore the available models.

Click on the file to download it. 

### Step 2: Open a Command-Line Interface
Open a terminal (e.g., Terminal on a Mac) and navigate to the folder where your downloaded model is located, using the `cd` command. For example, this might be the "Downloads" folder on your Mac. In that case, the command would be:

```bash
cd Downloads
```

### Step 3: Change Permissions (Mac)

On Mac, you need to grant permission for executing this file. You only need to do this once. 

```bash
chmod +x <llamafile_model_file_name>
```

If you're a Windows user, checkout the [Llamafile GitHub page](https://github.com/Mozilla-Ocho/llamafile?tab=readme-ov-file#llamafile).


### Step 4: Run the Model
```bash
./<llamafile_model_file_name>
```

This will open a window in your default web browser under `http://127.0.0.1:8080`, allowing you to interact with the LLM through a chat interface.

## Ending the Llamafile Session

To end the Llamafile session, go back to your terminal and use the keyboard combination `Control`and `C`. This will stop the LLM from running. 

