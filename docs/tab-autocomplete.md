---
title: ✅ Tab Autocomplete
description: PearAI is the open-source autopilot for software development
keywords: [shortcuts, pearai, important shortcuts, pear ai shortcuts]
sidebar_position: 3
---

# ✅ Tab AutoComplete

PearAI supports tab autocomplete, which predicts and suggests what you would type next as you're coding. Here's how to set it up:

## Setup Guide

1. **Setup Codestral**

   We recommend using [Codestral](https://mistral.ai/news/codestral/), the leading model for code completion (or FIM — Fill In Middle). It's also open-sourced! You'll need to obtain a Codestral API key from [Mistral API](https://console.mistral.ai).

2. **Add to PearAI config.json**

   Add the following to your config.json file (replace "YOUR_API_KEY" with your actual API key):

   ```json
   "tabAutocompleteModel": {
     "title": "Codestral",
     "provider": "mistral",
     "model": "codestral-latest",
     "apiKey": "YOUR_API_KEY"
   }

   ```

3. **Enjoy the development speed up with autocomplete!**

## Alternatives

- You can enhance your tab autocomplete with [Supermaven](https://supermaven.com/). It is currently one of the best autocomplete AI on the market, and provides a free tier. You can get started by installing Supermaven directly as an extension within PearAI.

  ![Supermaven extension](../static/img/supermaven.png)

- Additionally, you can use [Ollama](https://ollama.ai/) local models by downloading the desired model and adding it to your configuration.

  ```json
  "tabAutocompleteModel": {
      "title": "StarCoder2",
      "provider": "ollama",
      "model": "starcoder2:latest"
    },
    {
      "title": "Llama 3.2",
      "provider": "ollama",
      "model": "llama3.2:1b"
    },
    {
      "title": "Qwen 2.5 Coder",
      "provider": "ollama",
      "model": "qwen2.5-coder:1.5b"
    }
  ```
