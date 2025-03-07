---
layout: post
title: "Logseq AI Todo List Generator"
date: 2025-03-04
---
## Description
Everytime the user opens up logseq first thing in the morning, it will populate with a todo list based on activity recorded in previous daily journals.

## Overview
Run a python script on windows task scheduler at sometime during the night to generate a *.md file in the journals folder for the next day. The script reaches out to a locally deployed pc running an llm model. I'm running a Llama3.2: 7B on a cheap mini pc on my home network.

## Stack
- Ollama
- Logseq
- Python 3.12
- Windows Task Scheduler

## Steps
    1. Setup Windows machine
    2. Download Ollama to speed up the deployment of pretrained AI models
    3. Set environment variable "OLLAMA_HOST" to the internal IP of your machine, in order to bind the service to that address for network communication.
    4. If on windows, either add ollama installation folder to the PATH variable or navigate to installation directory and launch a model using ollama run [model name] ie "ollama run llama3.2:latest".
    5. Create firewall rule to allow for communication over port 11434.
    6. Install logseq on laptop or pc on the network.
    7. Use Windows task scheduler to efficiently run the python script at 1am every night.
    8. Wake up to a populated todo list to help remind you of things that need to be done!
