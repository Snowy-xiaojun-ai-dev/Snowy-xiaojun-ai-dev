# Hi there, I'm 梁家俊 (Snowy) 

专注大模型应用落地、RAG 检索优化与模型私有化部署。拥有从底层模型微调、端侧量化部署，到高级 RAG 架构设计的全栈工程经验。

##  核心项目展示

### 1. 企业级双引擎智能知识中枢 (Modular RAG System)
 **[项目代码仓库](https://github.com/Snowy-xiaojun-ai-dev/capstone_project)**
*   **技术栈**: LlamaIndex, 智谱GLM-4, BGE-Embedding, Gradio, Python.
*   **项目亮点**: 
    *   摒弃传统单库 RAG，采用**多库隔离 + 智能路由分发**架构，彻底解决企业垂直领域“查不准”的痛点。
    *   通过 `OpenAILike` 接口无缝接入云端大模型，结合定制化强约束 Prompt，完美解决小模型长上下文提取时的“过度解释”与“幻觉”问题。
    *   沉淀了完整的微调实验、系统架构图与数万字的踩坑反思记录。

### 2. 垂直领域 LoRA 微调与端侧部署
*   **技术栈**: LLaMA-Factory, Qwen2-0.5B, Ollama, GGUF.
*   **项目亮点**: 完整验证了从 Alpaca 格式数据清洗、LoRA 微调、GGUF 4-bit 量化到 Ollama 本地私有化部署的全流程。

##  技术栈
- **大模型**: LLaMA-Factory, LoRA/QLoRA, Ollama, GGUF 转换
- **RAG/检索**: LlamaIndex, LangChain, Chroma, BM25, RRF, LLMLingua
- **语言/框架**: Python, FastAPI, Gradio

##  联系我
- GitHub: [@Snowy-xiaojun-ai-dev](https://github.com/Snowy-xiaojun-ai-dev)
