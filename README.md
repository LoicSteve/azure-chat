# azure-chat

# Azure Chat Demo
Examples to use Azure with LLMs for Chat and learn how to use Azure OpenAI Service to create powerful AI-powered chat applications.

## Install the prerequisites

Use the `requirements.txt` to install all dependencies

```bash
python -m venv .venv
./.venv/bin/pip install -r requirements.txt
```

### Add your keys

Find the Azure OpenAI Keys in the Azure OpenAI Service. Note, that keys aren't in the studio, but in the resource itself. Add them to a local `.env` file. This repository ignores the `.env` file to prevent you (and me) from adding these keys by mistake.

Your `.env` file should look like this:

```
# Azure OpenAI 
OPENAI_API_TYPE="azure"
OPENAI_API_BASE="https://demo-steve-openai.openai.azure.com/"
OPENAI_API_KEY="your_api_key"
OPENAI_API_VERSION="2023-07-01-preview"

# Azure Cognitive Search
AZURE_COGNITIVE_SEARCH_SERVICE_NAME="https://demo-steve.search.windows.net"
AZURE_COGNITIVE_SEARCH_API_KEY="your_api_key"
AZURE_COGNITIVE_SEARCH_INDEX_NAME="demo-index"
```

Note that the Azure Cognitive Search is only needed if you are following the Retrieval Augmented Guidance (RAG) demo. It isn't required for a simple Chat application.
