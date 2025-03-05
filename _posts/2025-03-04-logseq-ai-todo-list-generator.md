---
layout: post
title: "Logseq AI Todo List Generator"
date: 2025-03-04
---

## Logseq AI Todo List Generator
# Use
    Everytime you open up logseq first thing in the morning, it will populate with a todo list based on activity recorded in previous daily journals.

# Description
     Run a python script on windows task scheduler at sometime during the night to generate a *.md file in the journals folder for the next day. The script reaches out to a locally deployed pc running an llm model. I'm running a Llama3.2: 7B on a cheap mini pc on my home network.

# Stack
    - Ollama
    - Logseq
    - Python 3.12
    - Windows Task Scheduler

# Instructions