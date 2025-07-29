# Welcome
This repo is a work-in-progress compilation of my samples based on [Azure OpenAI Service](https://learn.microsoft.com/en-us/azure/ai-services/openai/overview) and [OpenAI API](https://openai.com/api/) offered models. These samples are intended to simply convey the concepts and capabilities with code samples that are concise but sufficient to show how Generative AI can be applied to real-world scenarios.

# Azure OpenAI or OpenAI
I will mostly be using the common OpenAI Python SDK that supports both Azure OpenAI and OpenAI. 

For the service endpoint and credentials, I will use Azure OpenAI service and credentials for the most part because it's personally convenient. Regardless, the features and samples are applicable to both services.

# Setup

## Python Environment
This repository requires Python 3.8 or higher. To set up the environment:

### Option 1: Install core dependencies only
```bash
pip install -r requirements.txt
```

### Option 2: Install exact versions (reproducible environment)
```bash
pip install -r requirements-lock.txt
```

## Environment Variables
Most samples require environment variables for API keys and endpoints. You can either:
1. Set them in your system environment
2. Create `.env` files in the respective sample directories (recommended)

See individual sample directories for specific configuration requirements.


# List

1. **Functions**: Showcases the new "functions" feature with a simple example that transforms the user input into pre-defined functions invoked from the code, and the output sent back to GPT to get a natural language response, completing the semantic-syntactical-semantic loop.
1. **Extraction**: A variation on the OpenAI extraction example that adds numeric data to the input and CSV formatted response, loads it into a dataframe and plots it as a line chart.
1. **LangChain**: How to use LangChain with Azure OpenAI focusing on the new multiple tools feature and optionally disabling the parallel tools calling.