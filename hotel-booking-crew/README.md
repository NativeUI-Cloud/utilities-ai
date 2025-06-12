# Build a multi-agent hotel booking crew using DeepSeek-R1

In this tutorial we are building a 100% local multi-agent hotel booking crew. It find the cheapest and best hotels for you and uses DeepSeek-R1 running locally.

It features [Browserbase](https://dub.sh/bb1) to create a headless browser tool for the agents and CrewAI for multi-agent orchestration.

### Setup

To sync dependencies, run:

```sh
uv sync
```
    
### Environment Variables

You need to set up the following environment variables:

```sh
BROWSERBASE_API_KEY=...
OPENAI_API_KEY=... (not required for locally running)
```
[Get your browser base API key here](https://dub.sh/bb1)

OpenAI API key needed only when you are running app_openai.py. app.py uses a locally running DeepSeek with Ollama. ([how to setup local llm](https://ollama.com/library/deepseek-r1))

Ensure these variables are configured correctly before running the application use `.env.example` as reference and create your own `.env` file.

Run the streamlit app using `streamlit run app.py`

---
