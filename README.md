# llama.cpp server (CUDA) - Docker Compose

This compose file runs the `ghcr.io/ggml-org/llama.cpp:server-cuda` image exposing port 8080.

Usage

1. Place your model file under `./models` (e.g. `./models/ggml-model.bin`).

```sh
curl -L https://huggingface.co/unsloth/Qwen3.6-35B-A3B-GGUF/resolve/main/Qwen3.6-35B-A3B-UD-IQ1_M.gguf?download=true -o ./models/Qwen3.6-35B-A3B-UD-IQ1_M.gguf
```

2. Start the container:

```bash
docker compose up -d
```

3. Stop the container:

```bash
docker compose down
```

## System specs

- 13th Gen Intel Core i7-13700K 16 cores at 3.40GHz
- 32 GB of DDR5 RAM
- GeForce RTX 4060 8GB VRAM
