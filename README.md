# LLM-Powered Document Editor: DSPy & LangChain Integration for Intelligent Writing (OpenAI/Deepseek/Gemini/Github)

**An intelligent writing assistant with multi-LLM integration for enhanced content creation and editing.**

[![Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://doc-editor.streamlit.app)

[![App Screen Recording](https://github.com/user-attachments/assets/9adbdbc6-2138-4d63-8e0e-83dd8cb03d7f)](https://github.com/user-attachments/assets/f37c4dd5-423c-4406-a08d-51f67942ac7b)

Leverage DSPy's LLM orchestration and LangChain's document processing to create, refine, and manage content with unprecedented efficiency. Ideal for technical writers, content creators, and knowledge workers seeking intelligent document editing.

## 📚 Table of Contents
- [LLM-Powered Document Editor: DSPy \& LangChain Integration for Intelligent Writing (OpenAI/Deepseek/Gemini/Github)](#llm-powered-document-editor-dspy--langchain-integration-for-intelligent-writing-openaideepseekgeminigithub)
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

3. Configure environment:
```
cp .env.example .env  # Implement environment template
```

4. Add your API key (either one required):
```
OPENAI_API_KEY=your_openai_api_key
DEEPSEEK_API_KEY=your_deepseek_api_key
GEMINI_API_KEY=your_gemini_api_key
GITHUB_TOKEN=your_github_token
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

- **Quality Control**
  - 🔍 Semantic feedback tracking with source references
  - 📊 Real-time feedback dashboard

### 3. Finalization & Management
- **Output Optimization**
  - 🧮 Batch operation processing for bulk edits
  - 📖 Focus-optimized read mode

- **Advanced Orchestration**
  - 🚦 DSPy-managed suggestion pipeline
  - 📜 Version history tracking
  - 🌐 Multi-modal previews (raw + rendered views)

## ⚙️ System Architecture

[![](https://mermaid.ink/img/pako:eNqdVV1r2zAU_SvCpWODmGUrpKkfBknsjMEKZW4oDL8o9o0tYusaSW4a2v73XVv-iLvuYdGTPu45urrnSHp2YkzA8Zxdjoc448qwez-SjNrlJbvlQrIVFiVKkEbb-Y0G9TFydtzbcbeiAXtQwoCKnE82IEiEwSEEaMhCo4AXOfU2P_rAB1R7XfIY-tiEG77lGoYlQnIDPcQP74599FbV-dVT7E5hDFrjkMVPLtNVRgF9eC7kfphmYUnpnOa9Bki2PN73gBiLoj53v8LCozZQ9IiwKgquhoR2IgeX56ZbYIFMhRyyD55KVGY4LR5kjjxp59ktJlVuo3sJViglxEagPCk_c91vLx0LVwoPrhJpZqwS-nOtgI6cl1aKU1lGUM0fgS0qg01PM4M1qK_9G5XGUPIKsHvaNgXV7NXo8GEo8BsZRui4Mrb-tCc8GfYoeE3Rlm2QegQqeCpi9h0kKLJEs2cnzFjAEaqSCbJNmXSQN6frlBplh-WRfIfqXcQ_6nGUMfsFO8Jk8Fft38c0dgGrvbWA7iphhyc-CM2R_JuygzAZOxBdfWFdXUIsdlSVGHNUrUM0hUInN-2Rexc30yC4mU60UbgH7-Lq6qrtuweRmMz7Wj5NGgrvYtq0U6YheUs2v14FwfJMskZVy7NeL2erL2fyDL7qyBbT68WZZL1xLJfvL6a-fyZXZ6g2rWkwm6_OpGqfhVbC-Xp5Mz-TqXk0LE8wC2br_ymUM3EKUAUXCX0TzzVr5JgMCnqoPOomXO0jJ5KvFMfpKQnpIjieURVMHIVVmjlk9VzTqGouoS94qnjRz5Zc_kYcxtD49tb-Ss3n9PoHw9cvYQ?type=png)](https://mermaid.live/edit#pako:eNqdVV1r2zAU_SvCpWODmGUrpKkfBknsjMEKZW4oDL8o9o0tYusaSW4a2v73XVv-iLvuYdGTPu45urrnSHp2YkzA8Zxdjoc448qwez-SjNrlJbvlQrIVFiVKkEbb-Y0G9TFydtzbcbeiAXtQwoCKnE82IEiEwSEEaMhCo4AXOfU2P_rAB1R7XfIY-tiEG77lGoYlQnIDPcQP74599FbV-dVT7E5hDFrjkMVPLtNVRgF9eC7kfphmYUnpnOa9Bki2PN73gBiLoj53v8LCozZQ9IiwKgquhoR2IgeX56ZbYIFMhRyyD55KVGY4LR5kjjxp59ktJlVuo3sJViglxEagPCk_c91vLx0LVwoPrhJpZqwS-nOtgI6cl1aKU1lGUM0fgS0qg01PM4M1qK_9G5XGUPIKsHvaNgXV7NXo8GEo8BsZRui4Mrb-tCc8GfYoeE3Rlm2QegQqeCpi9h0kKLJEs2cnzFjAEaqSCbJNmXSQN6frlBplh-WRfIfqXcQ_6nGUMfsFO8Jk8Fft38c0dgGrvbWA7iphhyc-CM2R_JuygzAZOxBdfWFdXUIsdlSVGHNUrUM0hUInN-2Rexc30yC4mU60UbgH7-Lq6qrtuweRmMz7Wj5NGgrvYtq0U6YheUs2v14FwfJMskZVy7NeL2erL2fyDL7qyBbT68WZZL1xLJfvL6a-fyZXZ6g2rWkwm6_OpGqfhVbC-Xp5Mz-TqXk0LE8wC2br_ymUM3EKUAUXCX0TzzVr5JgMCnqoPOomXO0jJ5KvFMfpKQnpIjieURVMHIVVmjlk9VzTqGouoS94qnjRz5Zc_kYcxtD49tb-Ss3n9PoHw9cvYQ)

## 🔧 Technical Stack

| Component       | Technology       | Purpose                    |
|-----------------|------------------|----------------------------|
| AI Framework    | DSPy             | LLM operations management |
| Text Processing | LangChain        | Document chunking          |
| UI Framework    | Streamlit        | Web interface              |

## 📄 License

MIT Licensed - See [LICENSE](LICENSE) for details.
