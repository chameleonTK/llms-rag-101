# LLM & RAGs 101

Resources and hands-on labs for the **LLM & RAGs 101** seminar. The material introduces large language models, embeddings, retrieval-augmented generation (RAG), ReAct agents, and vectorless RAG.

## Requirements

- Python 3.11 or later
- [uv](https://docs.astral.sh/uv/)
- A Google Gemini API key
- Git, for downloading the dataset used in the labs

## Setup

Clone the repository and install the dependencies defined in `pyproject.toml`:

```bash
uv sync
```

Create your local environment file from the provided template:

```bash
cp .env.example .env
```

Get a Gemini API key from [Google AI Studio](https://aistudio.google.com/), then add it to `.env`:

```dotenv
GEMINI_KEY="your-api-key"
```

The `.env` file is ignored by Git. Do not commit API keys or other secrets.

Download the dataset used by the embedding and RAG labs:

```bash
git clone https://github.com/Pittawat2542/krathu-500.git
```

Start JupyterLab from the project environment:

```bash
uv run --with jupyter jupyter lab
```

## Labs

| Lab | Topic | Notebook |
| --- | --- | --- |
| 1 | Getting started with LLMs and LangGraph | `Lab1 Get Started.ipynb` |
| 2 | Embeddings | `Lab2 Embeddings.ipynb` |
| 3 | Simple RAG | `Lab3.1 Simple RAG.ipynb`, `Lab3.2 Simple RAG.ipynb` |
| 4 | ReAct agents | `Lab4 ReAct Agent.ipynb` |
| 5 | Vectorless RAG | `Lab5.1 Vecterless RAG.ipynb`, `Lab5.2 Vecterless RAG.ipynb` |

The `v1/` directory contains material from the earlier version of the seminar.

## Author

Pakawat Nakwijit — [pakawat.nk@gmail.com](mailto:pakawat.nk@gmail.com)
