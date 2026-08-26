# llllm-pipecat 🐝

Fork of [llllm](https://github.com/AaratiAkkapeddi/llllm) with the addition of voice/audio via [pipecat](https://github.com/pipecat-ai/pipecat)

## dependencies
- Python >=3.11
- [`uv`](https://docs.astral.sh/uv/getting-started/installation/)
- macOS M4 
	- (for MLXModel. TODO: make this more platform agnostic/friendly... keep an eye on [locat](https://github.com/vipyne/locat) for that)

## setup

```bash
cp .env.example .env
```
update the environment variables to where local models should live

```bash
uv sync
```

## run

```bash
uv run bot.py
```

the first run will take a little longer before starting (to download models and to build the rag embeddings). subsequent runs should be snappier.
