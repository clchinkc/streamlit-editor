# LLM-Powered Document Editor: DSPy & LangChain Integration for Intelligent Writing (OpenRouter/OpenAI/Deepseek/Gemini/Github/Ollama)

[![X URL](https://img.shields.io/twitter/url/https/x.com/firstoryapp.svg?style=social&label=Follow%20%40firstoryapp)](https://x.com/firstoryapp)
[![Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://doc-editor.streamlit.app)

**An intelligent writing assistant with multi-LLM integration for enhanced content creation and editing.**

[![App Screen Recording](https://github.com/user-attachments/assets/9adbdbc6-2138-4d63-8e0e-83dd8cb03d7f)](https://github.com/user-attachments/assets/f37c4dd5-423c-4406-a08d-51f67942ac7b)

Leverage DSPy's LLM orchestration and LangChain's document processing to create, refine, and manage content with unprecedented efficiency. Ideal for technical writers, content creators, and knowledge workers seeking intelligent document editing.

## 📚 Table of Contents
- [LLM-Powered Document Editor: DSPy \& LangChain Integration for Intelligent Writing (OpenRouter/OpenAI/Deepseek/Gemini/Github/Ollama)](#llm-powered-document-editor-dspy--langchain-integration-for-intelligent-writing-openrouteropenaideepseekgeminigithubollama)
  - [📚 Table of Contents](#-table-of-contents)
  - [🚀 Quick Start](#-quick-start)
  - [✨ Intelligent Document Workflows](#-intelligent-document-workflows)
    - [1. Content Creation Phase](#1-content-creation-phase)
    - [2. AI Collaboration Phase](#2-ai-collaboration-phase)
    - [3. Finalization \& Management](#3-finalization--management)
  - [⚙️ System Architecture](#️-system-architecture)
  - [🔧 Technical Stack](#-technical-stack)
  - [📄 License](#-license)

## 🚀 Quick Start

Try the live demo immediately:
[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://doc-editor.streamlit.app)

1. Clone repository:
```
git clone https://github.com/clchinkc/streamlit-editor.git
python -m venv venv
source venv/bin/activate  # Unix/MacOS
# .\venv\Scripts\activate  # Windows
```

2. Install dependencies:
```
pip install -r requirements.txt
```

3. Configure Streamlit secrets:
```bash
mkdir -p .streamlit
touch .streamlit/secrets.toml
```

Add the following to `.streamlit/secrets.toml`:
```toml
# API Keys (at least one required)
[openrouter]
OPENROUTER_API_KEY = "your_openrouter_api_key"
OPENROUTER_MODEL = "your_openrouter_model"

[openai]
OPENAI_API_KEY = "your_openai_api_key"

[deepseek]
DEEPSEEK_API_KEY = "your_deepseek_api_key"

[gemini]
GEMINI_API_KEY = "your_gemini_api_key"

[github]
GITHUB_TOKEN = "your_github_token"

[ollama]
OLLAMA_MODEL = "your_ollama_model"
```

4. (If you want to use Ollama) Setup Ollama:

First, install [Ollama](https://ollama.com/download).

Then start Ollama server with the specified model:
```
ollama run your_ollama_model
```

5. Launch application:
```
streamlit run streamlit_editor.py
```
And the app will be running on http://localhost:8501.

## ✨ Intelligent Document Workflows

**Combined Features & User Processes**

### 1. Content Creation Phase
- **Multi-format Editing Suite**
  - ✍️ Dual-mode editor (Editor + Markdown Preview)
  - 📥 File ingestion: Drag-and-drop `.md`/`.txt` support
  - 📤 Export flexibility: Download markdown or clipboard copy
  
- **Structural Tools**
  - 🗂️ LangChain-powered document chunking
  - 📚 Section-level editing

### 2. AI Collaboration Phase
- **Context-Aware Assistance**
  - 🤖 DSPy-powered feedback suggestions (general or specific to reference text)
  - 📑 Automated section summarization
  - 🧩 LLM-driven content regeneration
  - 📝 Review and compare AI-generated changes

- **Quality Control**
  - 🔍 Semantic feedback tracking with source references
  - 📊 Real-time feedback dashboard
  - ✅ Accept/reject AI suggestions with diff view

### 3. Finalization & Management
- **Output Optimization**
  - 🧮 Batch operation processing for bulk edits

- **Advanced Orchestration**
  - 🚦 DSPy-managed suggestion pipeline
  - 📜 Version history tracking
  - 🌐 Multi-modal previews (raw + rendered views)
  - 📄 Pagination for summaries

## ⚙️ System Architecture

[![](https://mermaid.ink/img/pako:eNqdVV1r2zAU_SvCpWODmGUrpKkfBknsjMEKZW4oDL8o9o0tYusaSW4a2v73XVv-iLvuYdGTPu45urrnSHp2YkzA8Zxdjoc448qwez-SjNrlJbvlQrIVFiVKkEbb-Y0G9TFydtzbcbeiAXtQwoCKnE82IEiEwSEEaMhCo4AXOfU2P_rAB1R7XfIY-tiEG77lGoYlQnIDPcQP74599FbV-dVT7E5hDFrjkMVPLtNVRgF9eC7kfphmYUnpnOa9Bki2PN73gBiLoj53v8LCozZQ9IiwKgquhoR2IgeX56ZbYIFMhRyyD55KVGY4LR5kjjxp59ktJlVuo3sJViglxEagPCk_c91vLx0LVwoPrhJpZqwS-nOtgI6cl1aKU1lGUM0fgS0qg01PM4M1qK_9G5XGUPIKsHvaNgXV7NXo8GEo8BsZRui4Mrb-tCc8GfYoeE3Rlm2QegQqeCpi9h0kKLJEs2cnzFjAEaqSCbJNmXSQN6frlBplh-WRfIfqXcQ_6nGUMfsFO8Jk8Fft38c0dgGrvbWA7iphhyc-CM2R_JuygzAZOxBdfWFdXUIsdlSVGHNUrUM0hUInN-2Rexc30yC4mU60UbgH7-Lq6qrtuweRmMz7Wj5NGgrvYtq0U6YheUs2v14FwfJMskZVy7NeL2erL2fyDL7qyBbT68WZZL1xLJfvL6a-fyZXZ6g2rWkwm6_OpGqfhVbC-Xp5Mz-TqXk0LE8wC2br_ymUM3EKUAUXCX0TzzVr5JgMCnqoPOomXO0jJ5KvFMfpKQnpIjieURVMHIVVmjlk9VzTqGouoS94qnjRz5Zc_kYcxtD49tb-Ss3n9PoHw9cvYQ?type=png)](https://mermaid.live/edit#pako:eNqdVV1r2zAU_SvCpWODmGUrpKkfBknsjMEKZW4oDL8o9o0tYusaSW4a2v73XVv-iLvuYdGTPu45urrnSHp2YkzA8Zxdjoc448qwez-SjNrlJbvlQrIVFiVKkEbb-Y0G9TFydtzbcbeiAXtQwoCKnE82IEiEwSEEaMhCo4AXOfU2P_rAB1R7XfIY-tiEG77lGoYlQnIDPcQP74599FbV-dVT7E5hDFrjkMVPLtNVRgF9eC7kfphmYUnpnOa9Bki2PN73gBiLoj53v8LCozZQ9IiwKgquhoR2IgeX56ZbYIFMhRyyD55KVGY4LR5kjjxp59ktJlVuo3sJViglxEagPCk_c91vLx0LVwoPrhJpZqwS-nOtgI6cl1aKU1lGUM0fgS0qg01PM4M1qK_9G5XGUPIKsHvaNgXV7NXo8GEo8BsZRui4Mrb-tCc8GfYoeE3Rlm2QegQqeCpi9h0kKLJEs2cnzFjAEaqSCbJNmXSQN6frlBplh-WRfIfqXcQ_6nGUMfsFO8Jk8Fft38c0dgGrvbWA7iphhyc-CM2R_JuygzAZOxBdfWFdXUIsdlSVGHNUrUM0hUInN-2Rexc30yC4mU60UbgH7-Lq6qrtuweRmMz7Wj5NGgrvYtq0U6YheUs2v14FwfJMskZVy7NeL2erL2fyDL7qyBbT68WZZL1xLJfvL6a-fyZXZ6g2rWkwm6_OpGqfhVbC-Xp5Mz-TqXk0LE8wC2br_ymUM3EKUAUXCX0TzzVr5JgMCnqoPOomXO0jJ5KvFMfpKQnpIjieURVMHIVVmjlk9VzTqGouoS94qnjRz5Zc_kYcxtD49tb-Ss3n9PoHw9cvYQ)

## 🔧 Technical Stack

| Component       | Technology        | Purpose                    |
|----------------|-------------------|----------------------------|
| AI Framework   | DSPy             | LLM operations management  |
| Text Processing| LangChain        | Document chunking          |
| UI Framework   | Streamlit        | Web interface              |
| Visualization  | Streamlit Mermaid| Document flow diagrams     |

## 📄 License

MIT Licensed - See [LICENSE](LICENSE) for details.
