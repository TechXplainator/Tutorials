# How to Build Free AI Agents - Minions for World Dominiation

In this tutorial, we're going to build AI agents on Google Colab with the help of LLaMA3 powered by Ollama and CrewAI. 

With these powerful tools, you can automate tasks that would normally take hours or days, such as preparing for meetings, generating customized trip plans, or writing blogs and social media posts. 

The good news is that this process is entirely free!

If you prefer learning through a visual approach or want to gain additional insight into this topic, be sure to check out my YouTube video on this subject!

[![install-ollama-thumbnail](/ai-agents/how-to-build-free-ai-agents-minions/ollama-agents-minions-thumbnail.png)](https://youtu.be/YA5hT4iFUIk)

## Quick Links

* Jupyter Notebooks
    * [Minions for world domination](/ai-agents/how-to-build-free-ai-agents-minions/world_domination.ipynb)
* Ngrok
	* [Ngrok website](https://ngrok.com/)
* Ollama
	* [Ollama website](https://ollama.com/)
	* [How to install Ollama locally](/ollama/install-ollama/README.md)
    * [How to run Ollama on Google Colab](/ollama/ollama-on-colab/README.md)
* Google Colab
	* [Google Colab website](https://colab.research.google.com/)
* CrewAI
    * [Website](https://www.crewai.com/)    
    * [Documentation](https://docs.crewai.com/)

## Setup

Here's what I'll be using:

* [Ollama](https://ollama.com/): framework for running large language models locally
	+ Open-source and easy to set up
	+ [Link](/ollama/install-ollama/README.md) for installation process
* [Google Colab](https://colab.research.google.com/): cloud-based platform for Python code 
	+ Free account required, assuming you already have one
* [Ngrok](https://ngrok.com/): gives local web applications a public URL
	+ Sign up for free account in description


## Setup Steps

1. [Expose local Ollama to public URL provided by Ngrok](#step-1---expose-local-ollama-to-public-url-provided-by-ngrok)
2. [Open and run a pre-prepared Jupyter Notebook on Colab, logged in with Google account.](#step-2-open-and-run-a-prepared-jupyter-notebook)
3. [Execute the code in Jupyter Notebook](#step-3-execute-jupyter-notebook)


### Step 1 - Expose local Ollama to public URL provided by Ngrok

When it comes to exposing Llama3 to Google Colab with Ngrok, you have two viable options. One approach is to install Ngrok on your machine and map your URL - a very straightforward process! Alternatively, you can run Llama3 on Colab using a Ngrok URL, without any installation of Ngrok to your local machine. You would choose the second option if (like me) you don't have enough GPU to run LLMs locally on your machine.

#### Option 1 - Install Ngrok and Expose your local URL

On your local machine:
 * Install ngrok: https://ngrok.com/download
 * Open a terminal and run: `ngrok http http://localhost:11434`
 * Copy the forwarding URL (it will be something like https://1234-your-ngrok-url.ngrok.io)

#### Option 2 - Run llama3 on Google Colab using Ngrok

I created a comprehensive tutorial that utilizes a static URL from Ngrok, allowing you to reuse it multiple times. You can find the tutorial here: [Running Ollama on Google Colab](/ollama/ollama-on-colab/README.md).


### Step 2: Open and run a prepared Jupyter Notebook

* Open this [Jupyter notebook](/ai-agents/how-to-build-free-ai-agents-minions/world_domination.ipynb) in Google Colab
* Ensure logged in with Google account first
* Navigate to "Secrets" section within Colab
* Add new secret and name it `OLLAMA_BASE_URL`. Now add the Ngrok URL from [step 1](#step-1---expose-local-ollama-to-public-url-provided-by-ngrok) as a value. 
* Add new secret called `OLLAMA_MODEL` and insert the name of the model you want to use via Ollama. In our case, it's `llama3`.
* Don't forget to enable notebook access for both values!

If you're intrested in a walkthrough of the Jupyter notebook, check out this [section](#jupyter-notebook-walkthrough).

### Step 3: Execute Jupyter Notebook

* Run all cells in the notebook
* You should see a printed output of your crew's work.

## Jupyter Notebook Walkthrough

### Installing Required Packages

* Install CrewAI framework and service for building and running complex multi-agent systems
* Import necessary modules and libraries, including Agent, Task, Crew, Process, Ollama, and userdata from Google Colab

```python
%pip install -q crewai
```

```python
# Download required packages
from crewai import Agent, Task, Crew
from crewai.process import Process
from langchain.llms import Ollama
from google.colab import userdata
```

### Initializing Ollama Language Model

* Define API keys and important values from Jupyter secrets section of Ollama
* Set base URL and model for the language model using `OLLAMA_BASE_URL` and `OLLAMA_MODEL`
* Initialize an Ollama language model by setting its base URL and model, and storing it in a variable called "llm"

```python
# Get API keys and variables from Jupyter secrets. Make sure to store these in the "secrets" section of Colab!
OLLAMA_BASE_URL = userdata.get('OLLAMA_BASE_URL')
OLLAMA_MODEL = userdata.get('OLLAMA_MODEL')
```

```python
# Initialize the LLM using Ollama
llm = Ollama(
    model = OLLAMA_MODEL,
    base_url = OLLAMA_BASE_URL
)
```

### Defining Agents

* Define agents with roles, goals, and backstories using natural language prompts
* Specify the large language model (LLM) to use for each agent
* Control delegation and verbosity of agents' internal workings


```python
# Define minion agents
mastermind = Agent(
    role="Evil Genius Mastermind",
    goal="Develop a grand strategy for world domination",
    backstory="You are the brilliant leader of the minions, always scheming to take over the world. Your plans are elaborate and often involve bananas.",
    allow_delegation = False,
    llm=llm,
    verbose=False
)

gadgeteer = Agent(
    role="Minion Gadget Inventor",
    goal="Create outrageous and somewhat functional gadgets for world domination",
    backstory="You're the creative genius behind all minion technology. Your inventions are as unpredictable as they are yellow.",
    llm=llm,
    allow_delegation = False,
    verbose=False
)

henchman = Agent(
    role="Chief Henchman",
    goal="Organize and motivate the minion army for world conquest",
    backstory="You're the minion's minion, capable of translating 'banana' into actionable plans. Your organizational skills are as impressive as your overalls.",
    llm=llm,
    allow_delegation = False,
    verbose=False
)

propagandist = Agent(
    role="Minion Propagandist",
    goal="Spread pro-minion sentiment across the globe",
    backstory="Your memes are legendary, your slogans catchy, and your ability to make world domination sound appealing is unmatched.",
    llm=llm,
    allow_delegation = False,
    verbose=False
)
```


### Creating Tasks

* Define tasks for each agent:
	+ Develop a grand strategy for world domination (Mastermind)
	+ Invent key gadgets for conquering the world (Gadgeteer)
	+ Create a training and deployment plan for the minion army (Henchman)
	+ Develop a global propaganda campaign to win hearts and minds (Propagandist)

```python
# Define tasks
strategy_task = Task(
    description="Develop a comprehensive strategy for world domination. Include key phases and targets.",
    agent=mastermind,
    expected_output="A detailed plan for world domination, minion-style."
)

gadget_task = Task(
    description="Invent three key gadgets crucial for the world domination plan. Describe their function and hilarious side effects.",
    agent=gadgeteer,
    expected_output="Descriptions of three wacky but somehow effective gadgets for conquering the world."
)

army_task = Task(
    description="Create a training and deployment plan for the minion army based on the master strategy.",
    agent=henchman,
    expected_output="A comprehensive plan for preparing and utilizing the minion workforce in the quest for world domination."
)

propaganda_task = Task(
    description="Develop a global propaganda campaign to win hearts, minds, and bananas for the minion cause.",
    agent=propagandist,
    expected_output="A multi-platform propaganda strategy to make minion rule seem like the best thing since sliced bananas."
)
```



### Running the Crew

* Initialize a Crew object named `my_crew` by combining defined agents with their assigned tasks
* Set verbose parameter to control the level of detail printed to the console during the crew's operation
* Run the crew's assigned tasks and display the outcome

```python
# Create the crew
my_crew = Crew(
    agents=[mastermind, gadgeteer, henchman, propagandist],
    tasks=[strategy_task, gadget_task, army_task, propaganda_task],
    verbose=1,
    process=Process.sequential
)
```

```python
# Run the crew
result = my_crew.kickoff()
print(result)
```