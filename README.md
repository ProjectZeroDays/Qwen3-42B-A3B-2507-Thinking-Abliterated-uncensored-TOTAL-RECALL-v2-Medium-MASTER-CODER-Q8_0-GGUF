---
license: apache-2.0
library_name: transformers
language:
- en
- fr
- zh
- de
tags:
- programming
- code generation
- code
- codeqwen
- moe
- coding
- coder
- qwen2
- chat
- qwen
- qwen-coder
- Qwen3-30B-A3B-Thinking-2507
- Qwen3-30B-A3B
- mixture of experts
- 128 experts
- 8 active experts
- 256k context
- qwen3
- finetune
- brainstorm 20x
- brainstorm
- thinking
- reasoning
- uncensored
- abliterated
- qwen3_moe
- llama-cpp
- gguf-my-repo
base_model: DavidAU/Qwen3-42B-A3B-2507-Thinking-Abliterated-uncensored-TOTAL-RECALL-v2-Medium-MASTER-CODER
pipeline_tag: text-generation
---

# sumgai/Qwen3-42B-A3B-2507-Thinking-Abliterated-uncensored-TOTAL-RECALL-v2-Medium-MASTER-CODER-Q8_0-GGUF
This model was converted to GGUF format from [`DavidAU/Qwen3-42B-A3B-2507-Thinking-Abliterated-uncensored-TOTAL-RECALL-v2-Medium-MASTER-CODER`](https://huggingface.co/DavidAU/Qwen3-42B-A3B-2507-Thinking-Abliterated-uncensored-TOTAL-RECALL-v2-Medium-MASTER-CODER) using llama.cpp via the ggml.ai's [GGUF-my-repo](https://huggingface.co/spaces/ggml-org/gguf-my-repo) space.
Refer to the [original model card](https://huggingface.co/DavidAU/Qwen3-42B-A3B-2507-Thinking-Abliterated-uncensored-TOTAL-RECALL-v2-Medium-MASTER-CODER) for more details on the model.

## Use with llama.cpp
Install llama.cpp through brew (works on Mac and Linux)

```bash
brew install llama.cpp

```
Invoke the llama.cpp server or the CLI.

### CLI:
```bash
llama-cli --hf-repo sumgai/Qwen3-42B-A3B-2507-Thinking-Abliterated-uncensored-TOTAL-RECALL-v2-Medium-MASTER-CODER-Q8_0-GGUF --hf-file qwen3-42b-a3b-2507-thinking-abliterated-uncensored-total-recall-v2-medium-master-coder-q8_0.gguf -p "The meaning to life and the universe is"
```

### Server:
```bash
llama-server --hf-repo sumgai/Qwen3-42B-A3B-2507-Thinking-Abliterated-uncensored-TOTAL-RECALL-v2-Medium-MASTER-CODER-Q8_0-GGUF --hf-file qwen3-42b-a3b-2507-thinking-abliterated-uncensored-total-recall-v2-medium-master-coder-q8_0.gguf -c 2048
```

Note: You can also use this checkpoint directly through the [usage steps](https://github.com/ggerganov/llama.cpp?tab=readme-ov-file#usage) listed in the Llama.cpp repo as well.

Step 1: Clone llama.cpp from GitHub.
```
git clone https://github.com/ggerganov/llama.cpp
```

Step 2: Move into the llama.cpp folder and build it with `LLAMA_CURL=1` flag along with other hardware-specific flags (for ex: LLAMA_CUDA=1 for Nvidia GPUs on Linux).
```
cd llama.cpp && LLAMA_CURL=1 make
```

Step 3: Run inference through the main binary.
```
./llama-cli --hf-repo sumgai/Qwen3-42B-A3B-2507-Thinking-Abliterated-uncensored-TOTAL-RECALL-v2-Medium-MASTER-CODER-Q8_0-GGUF --hf-file qwen3-42b-a3b-2507-thinking-abliterated-uncensored-total-recall-v2-medium-master-coder-q8_0.gguf -p "The meaning to life and the universe is"
```
or 
```
./llama-server --hf-repo sumgai/Qwen3-42B-A3B-2507-Thinking-Abliterated-uncensored-TOTAL-RECALL-v2-Medium-MASTER-CODER-Q8_0-GGUF --hf-file qwen3-42b-a3b-2507-thinking-abliterated-uncensored-total-recall-v2-medium-master-coder-q8_0.gguf -c 2048
```
