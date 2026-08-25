## Set up
* run `uv venv --python 3.11`
* run `source .venv/bin/activate`
* run `uv pip install matplotlib openai ollama`
* run `uv run --with jupyter jupyter lab`
* install ollama https://ollama.com/download
* download models (see list of models here https://ollama.com/search)

```
ollama pull scb10x/typhoon2.5-qwen3-4b
ollama pull hf.co/typhoon-ai/typhoon2.5-qwen3-4b-gguf:Q4_K_M
ollama pull qwen3-vl:4b-instruct
```
<!-- ollama pull hf.co/mradermacher/typhoon2.5-qwen3-4b-GGUF:Q4_K_M -->


#### For Lab1
* run `uv pip install google-genai`


#### For Lab3
* run `uv pip install mlx-vlm mlx-hub torchvision`
* run `mlx-hub-cli --download mlx-community/Qwen3-VL-4B-Instruct-8bit`
* (Optional) run `uv pip install mlx-audio mlx-whisper`
* (Optional) run `brew install ffmpeg`
* run `python -m mlx_vlm server` to start MLX Server

#### For Lab5
* run `uv pip install langchain-ollama langgraph pydantic`

#### For Lab6
* run `uv pip install qdrant-client fastembed`
* run `docker run -p 6333:6333 qdrant/qdrant`