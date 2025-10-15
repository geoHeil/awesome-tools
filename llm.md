# LLM

## good content

- https://jax-ml.github.io/scaling-book/
- ocr
  - https://www.sergey.fyi/articles/gemini-flash-2 and https://www.runpulse.com/blog/why-llms-suck-at-ocr and https://blog.roboflow.com/florence-2-ocr/
- https://applied-llms.org/
- https://github.com/ray-project/llm-numbers
- https://github.com/KalyanKS-NLP/llm-engineer-toolkit
- https://koomen.dev/essays/horseless-carriages/ horseless carriages of AI
- https://github.com/mlabonne/llm-course


## prompts

- https://github.com/preset-io/promptimize
- simple prompt engineering training from anthropic https://docs.google.com/spreadsheets/d/19jzLgRruG9kjUQNKtCg1ZjdD6l6weA6qRXG5zLIAhC8/edit?gid=150872633#gid=150872633 (Anthropic's Prompt Engineering Interactive Tutorial [PUBLIC ACCESS])
- https://colab.research.google.com/drive/1OnIipRwuHOZbKHN0haHGD0OnckBGfzqx auto optimierung
- prompting frameworks
  - https://github.com/masci/banks
  - https://github.com/boundaryml/baml
- prompt techniques
  - CoRT chain of recursive thoughts https://github.com/PhialsBasement/Chain-of-Recursive-Thoughts

## tokenization

- https://github.com/openai/tiktoken

## vector databases

- https://github.com/facebookresearch/faiss
- https://www.pinecone.io/
- https://www.trychroma.com/

## hallucination
- https://docs.vectara.com/docs/learn/hallucination-evaluation


## private

- https://bdtechtalks.com/2023/06/01/create-privategpt-local-llm/amp/

## stacks
### serving LLMs

- https://github.com/ajndkr/lanarky
- https://github.com/deepset-ai/haystack (with Elasticsearch)

### full e2e example

- https://github.com/praj2408/Langchain-PDF-App-GUI

### ready made connectors

- https://www.danswer.ai/
- https://n8n.io/

## no code GUI tools

- https://github.com/FlowiseAI/Flowise
- https://github.com/gmpetrov/databerry
- https://www.docetl.org/

## models

- https://x.com/clementdelangue/status/1934672721066991908
- https://simonwillison.net/2024/Dec/24/qvq/
- https://simonwillison.net/2024/Dec/26/deepseek-v3/


## document preprocessors

- unstract.com LLM whisperer https://pg.llmwhisperer.unstract.com/
	- https://github.com/Zipstack/unstract
- https://cloud.llamaindex.ai llamaparse
- **https://github.com/DS4SD/docling**
- https://github.com/VikParuchuri/marker
- https://github.com/QuivrHQ/MegaParse
- https://github.com/microsoft/markitdown
- https://github.com/opendatalab/PDF-Extract-Kit

### HTML cleanup

- https://emschwartz.me/comparing-13-rust-crates-for-extracting-text-from-html/
### pdf preprocessors

- https://github.com/opendatalab/MinerU
- https://github.com/DS4SD/docling

### entity extraction

- https://python.useinstructor.com/
- https://github.com/vlm-run/vlmrun-cookbook and good comments https://news.ycombinator.com/item?id=43187209
- https://github.com/boundaryml/baml

#### naming entities

- https://github.com/urchade/GLiNER

## security

- https://github.com/NVIDIA/garak
- https://github.com/Azure/PyRIT
- https://www.promptfoo.dev/docs/red-team/quickstart/
- https://github.com/mbrg/power-pwn
- cryptography
  - https://eprint.iacr.org/2025/288
- prompt injection scanning
  - https://arstechnica.com/information-technology/2025/04/researchers-claim-breakthrough-in-fight-against-ais-frustrating-security-hole/ https://arxiv.org/abs/2503.18813
### scraper & automation

- https://github.com/browser-use/browser-use
- https://github.com/nanobrowser/nanobrowser

  
### jailbreaks

- https://github.com/CHATS-lab/persuasive_jailbreaker

### demonstrations

- https://github.com/greshake/llm-security
- https://bishopfox.com/resources/rvasec2024-patch-perfect-harmonizing-llms

### ethical challenges

- https://www.youtube.com/watch?v=giT0ytynSqg

### security problems

- https://theyseeyourphotos.com/
- https://www.404media.co/email/f459caa7-1a58-4f31-a9ba-3cb53a5046a4/
- https://www.npr.org/2024/12/10/nx-s1-5222574/kids-character-ai-lawsuit
- https://bsky.app/profile/pedram.lol/post/3lbxzc34th22y
- https://www.heise.de/news/Copilot-macht-aus-einem-Gerichtsreporter-einen-Kinderschaender-9840437.html
- https://github.com/leondz/garak
- https://www.youtube.com/watch?v=qyTSOSDEC5M
- https://gandalf.lakera.ai/baseline genAI security training
- https://www.heise.de/news/ChatGPT-Code-mit-betruegerischer-API-kostet-Programmierer-2500-US-Dollar-10169146.html
- https://microsoft.github.io/presidio/analyzer/
- https://www.promptfoo.dev/docs/red-team/quickstart/
- https://github.com/mbrg/power-pwn
- https://www.youtube.com/watch?v=-YJgcTCSzU0
- https://www.youtube.com/watch?v=LcLrG_4i19E
- https://www.youtube.com/watch?v=LcLrG_4i19E
- backdoor
  - https://blog.sshh.io/p/how-to-backdoor-large-language-models
 
- email summarization copiarate https://www.youtube.com/watch?v=84NVG1c5LRI
- uncensor with abliteration https://colab.research.google.com/drive/1VYm3hOcvCpbGiqKZb141gJwjdmmCcVpR?usp=sharing


identifying security issues

- graph aware scanning
  - https://hiddenlayer.com/innovation-hub/shadowgenes-uncovering-model-genealogy/
  - https://arxiv.org/abs/2501.11830
#### red teaming

- https://airedteamwhitepapers.blob.core.windows.net/lessonswhitepaper/MS_AIRT_Lessons_eBook.pdf
- https://www.microsoft.com/en-us/security/blog/2025/01/13/3-takeaways-from-red-teaming-100-generative-ai-products/
- https://github.com/Azure/PyRIT


### data poisoning

- https://arxiv.org/pdf/2302.04222 glaze
- https://arxiv.org/pdf/2310.13828 night shade
  - https://nightshade.cs.uchicago.edu/whatis.html

## fine-tuning

- https://huggingface.co/docs/peft/index
- https://github.com/unslothai/unsloth
- https://github.com/axolotl-ai-cloud/axolotl
- https://github.com/Lightning-AI/litgpt
- https://github.com/hiyouga/LLaMA-Factory
- tool lists
  - https://huyenchip.com/llama-police
- https://github.com/meta-llama/synthetic-data-kit
- https://pypi.org/project/tokenlearn/
- auto eval https://colab.research.google.com/drive/1Igs3WZuXAIv9X0vwqiE90QlEPys8e8Oa?usp=sharing
- axolotl https://colab.research.google.com/drive/1TsDKNo2riwVmU55gjuBgB1AXVtRRfRHW?usp=sharing
- unsloth https://colab.research.google.com/drive/164cg_O7SV7G8kZr_JXqLd6VC7pd86-1Z?usp=sharing

### newer efficient way of fine-tuning and distillation

SVD and Marchenko-Pastur seem to be really useful

- https://github.com/arcee-ai/DistillKit https://www.youtube.com/watch?v=JE7SuP049mQ
- https://github.com/cognitivecomputations/spectrum https://www.youtube.com/watch?v=CTncBjRgktk
- https://github.com/arcee-ai/mergekit
  - https://www.youtube.com/watch?v=cvOpX75Kz4M
  - https://www.youtube.com/watch?v=qbAvOgGmFuE
  - https://colab.research.google.com/drive/1obulZ1ROXHjYLn6PPZJwRR6GzgQogxxb?usp=sharing
- https://github.com/arcee-ai/EvolKit
- https://www.arcee.ai/blog/how-arcee-ai-helped-madeline-co-build-a-world-class-reasoning-model-from-first-principles- https://www.arcee.ai/product/arcee-conductor
 
## distributed training

- https://github.com/microsoft/DeepSpeed
- https://pytorch.org/tutorials/distributed/home.html
- https://lightning.ai/docs/pytorch/stable/
- https://github.com/hpcaitech/ColossalAI

## prototyping

### UIs

- https://github.com/open-webui/open-webui
- https://lmstudio.ai/
- https://opencat.app/en/
- https://docs.chainlit.io/get-started/overview
- https://www.gradio.app/
- https://streamlit.io/

## rag frameworks

- https://github.com/llmware-ai/llmware
- https://github.com/infiniflow/ragflow?tab=readme-ov-file
- https://github.com/Filimoa/open-parse
- rag tools
  - https://www.onyx.app/
- https://github.com/google-gemini/gemini-fullstack-langgraph-quickstart
- https://github.com/eyelevelai/groundx-on-prem
- https://github.com/morphik-org/morphik-core
- https://github.com/timescale/pgai

### graph rag

- https://github.com/Muvon/octocode

### rag applications

- https://arxiv.org/abs/2409.13740

## workflows

- https://workflowai.com/

## agents

- https://github.com/humanlayer/12-factor-agents
- https://github.com/The-Pocket/PocketFlow
- https://claudiacode.com/

### parallel agentic development

- https://conductor.build/

## verification & Testing

- 10.17323/jle.2020.11046


## education

### audio

- https://livekit.io/
- https://huggingface.co/Zyphra/Zonos-v0.1-hybrid
- https://github.com/nari-labs/dia
- https://github.com/KoljaB/RealtimeVoiceChat
- https://github.com/resemble-ai/chatterbox

### video

- explanation videos

## hosting models

- https://github.com/containers/ramalama
- https://ollama.com/
- https://github.com/vllm-project/vllm
- https://huggingface.co/moonshotai/Kimi-Audio-7B-Instruct
- https://github.com/sgl-project/sglang

## hardware

on demand AI clusters

- all the public cloud providers (though they often do not focus on offering a simple/streamlined GPU experience for researchers)
- https://hpc-ai.com
- https://lambdalabs.com/service/gpu-cloud/1-click-clusters
- https://vast.ai/
- https://www.paperspace.com
- https://huggingface.co/spaces
- https://colab.research.google.com/
- https://www.anyscale.com
- https://www.fluidstack.io

### validation of hardware
- check cooling issues
  - https://github.com/huggingface/gpu-fryer
- https://www.runpod.io/
  - https://github.com/3b1b/manim
- https://github.com/exo-explore/exo

## video generation

- https://github.com/Wan-Video/Wan2.2
## realtime
### audio

#### serving

- https://fastrtc.org/

#### models
- https://github.com/canopyai/Orpheus-TTS
- https://github.com/fixie-ai/ultravox
- https://www.openai.fm/
- qwen 2.5 omni
  - https://huggingface.co/spaces/Qwen/Qwen2.5-Omni-7B-Demo
  - https://huggingface.co/Qwen/Qwen2.5-Omni-7B
- https://zeyuet.github.io/AudioX/

#### solutions
- https://livekit.io/
- https://elevenlabs.io/

## data analysis with AI

- https://github.com/microsoft/data-formulator


## paper finders

- https://allenai.org/blog/paper-finder


## applications

### schooling and tutoring

- https://www.synthesis.com/tutor



## ai and politics

- religion
  - vatican AI rules https://www.vatican.va/roman_curia/congregations/cfaith/documents/rc_ddf_doc_20250128_antiqua-et-nova_en.html
 
## mcp

### registry

- https://github.com/IBM/mcp-context-forge


## applications

### observability

- https://github.com/Arize-ai/phoenix
