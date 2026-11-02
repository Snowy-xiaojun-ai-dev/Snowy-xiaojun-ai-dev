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

### 3. 企业级自反思智能体 (Agentic RAG & Auto-Evaluation)
    **[项目代码仓库](https://github.com/Snowy-xiaojun-ai-dev/Agent_RAG_project)**
*   **技术栈**: LangGraph, LlamaIndex, 智谱GLM-4, Tavily Search API, RAGAs, Streamlit.
*   **项目亮点**:
    *   **自主反思机制 (Self-Reflection)**：突破传统固定流程，采用 Agent 架构。大模型可自动评估检索质量，若召回失败，可自主触发“Query 改写”或“调用外部搜索引擎”进行补救（实测成功抓取实时天气数据）。
    *   **量化评估指标 (RAGAs)**：引入业界标准的评估框架，测试集跑分 **Faithfulness: 0.66, Answer Relevance: 0.80**，用数据客观验证了系统的可靠性。
    *   **安全工程化**：使用 `dotenv` 进行密钥隔离，防止 API Key 泄漏；前端采用 Streamlit 完整展示 Agent 的思维链（Chain of Thought）与决策路径。
### 4. 企业级多智能体协作营销系统 (Multi-Agent Marketing Crew)
    **[项目代码仓库](你刚生成的Multi_Agent仓库链接)**
*   **技术栈**: CrewAI, 智谱GLM-4 (Function Calling), Tavily Search, Python REPL.
*   **项目亮点**:
    *   **真实团队协作**：模拟市场调研员、产品专家、数据分析师、文案策划 4 个 AI 角色，按流水线自动接力完成工作。
    *   **动态工具调用**：Agent 自动评估任务需求，分别调用外部搜索引擎、本地知识库、Python 计算器，实现自动化闭环。
    *   **商业级产出**：仅输入一句模糊指令，系统自动生成具备数据支撑、痛点打击、情绪价值的“小红书爆款”种草推文。
### 5. 企业级 RAG 检索质量量化评估系统 (RAG Evaluation)
    **[项目代码仓库](https://github.com/Snowy-xiaojun-ai-dev/Enterprise_RAG_Evaluation)**
*   **技术栈**: LangChain, RAGAs, 智谱GLM-4, ChromaDB, BGE-Embedding.
*   **项目亮点**:
    *   **数据驱动优化**：构建 25+ 条自动化黄金测试集，引入 RAGAs 框架，彻底摆脱“凭感觉”评估，建立工业级 RAG 评测基线。
    *   **极致性能指标**：在真实演唱会规则文档下，基线跑分 **Context Recall 达到 1.0000**（100%精准召回），**Faithfulness 达到 0.9500**（极低幻觉率）。
    *   **工程排坑**：成功解决 LangChain Prompt 模板大括号转义冲突，并通过强约束 Prompt 大幅降低大模型回答的冗余度。
## 系统架构

`用户提问` -> `本地知识库检索` -> `[大模型自我反思]`
*   若命中 -> `生成最终答案`
*   若未命中 -> `触发 Tavily 联网搜索` -> `生成最终答案`

## 快速启动

1. 安装依赖：
   ```bash
   pip install langgraph langchain-openai tavily-python ragas streamlit python-dotenv langchain-huggingface
   
##  技术栈
- **大模型**: LLaMA-Factory, LoRA/QLoRA, Ollama, GGUF 转换
- **RAG/检索**: LlamaIndex, LangChain, Chroma, BM25, RRF, LLMLingua
- **语言/框架**: Python, FastAPI, Gradio

##  联系我
- GitHub: [@Snowy-xiaojun-ai-dev](https://github.com/Snowy-xiaojun-ai-dev)
