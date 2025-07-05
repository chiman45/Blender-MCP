
# 🌀 MCP Client & Blender Integration Suite

A comprehensive **Model Context Protocol (MCP)** implementation featuring:
- A **universal client** that can connect to any MCP server
- A specialized **Blender integration** tool for real-time 3D workflows powered by AI.

---

## 🚀 Features

### 🧠 Universal MCP Client (`mcp-client-python`)
- **Multi-LLM Support**: Seamless integration with Claude (Anthropic) and Gemini (Google)
- **FastAPI REST API**: Clean HTTP interface for external applications
- **Universal MCP Compatibility**: Connect to any MCP server following the MCP specification
- **Conversation Logging**: Automatic chat logging with JSON export
- **Robust Error Handling**: With detailed logs
- **CORS Support**: Ready for frontend/web integrations

### 🧩 Blender MCP Server (`blender-mcp`)
- **Direct Blender Integration**: Communicates with Blender via sockets in real-time
- **Asset Library Support**:
  - 🌄 **PolyHaven**: HDRIs, textures, and models
  - 🛒 **Sketchfab**: Download/import high-quality 3D models
  - 🧠 **Hyper3D Rodin**: AI-based 3D model generation from text or image prompts
- **Scene & Object Management**: Retrieve detailed object and scene data
- **Python Code Execution**: Run Python scripts directly inside Blender
- **Screenshot Capture**: Automatically capture Blender viewports
- **Material System**: Apply textures and materials to objects via API

---

## 🗂️ Project Structure






---

## 🛠️ Installation & Setup

### ✅ Prerequisites
- Python **3.8+**
- Blender **3.0+**
- API keys for:
  - Gemini (Google)
  - Claude (Anthropic)
  - PolyHaven
  - Sketchfab
  - Hyper3D

---

### ⚡ Quick Start

#### 1. Clone the repository
```bash
git clone https://github.com/yourusername/mcp-client-blender-suite.git
cd mcp-client-blender-suite
```
2. Set up the Universal MCP Client
```bash
cd mcp-client-python
pip install -r requirements.txt
```
3. Add API keys to .env file
```bash
echo "GEMINI_API_KEY=your_gemini_key_here" >> api/.env
echo "ANTHROPIC_API_KEY=your_claude_key_here" >> api/.env
```

4. Start the MCP client API
```bash
cd api
python main.py
# Server will run on http://localhost:8000
```

5. Install the Blender Addon
Open Blender → Edit > Preferences > Add-ons

Click "Install…" and select addon.py

Enable the addon and start the socket server via preferences

🎯 Use Cases
-🎨 3D Content Creation: Natural language commands for Blender tasks

-📦 Asset Management: Import assets from PolyHaven, Sketchfab, etc.

-🧠 AI-Powered Modeling: Generate 3D objects using text or image prompts

-⚙️ Workflow Automation: Run Python scripts and automate repetitive tasks

-📚 Educational Tool: Learn Blender with AI assistance

-🛠️ Rapid Prototyping: Build and test 3D concepts faster


🔌 API Endpoints
  -MCP Client API (FastAPI)
  -POST /query — Send a query to the connected MCP server

GET /tools — List available tools

🧠 AI model (Claude or Gemini) is auto-selected based on .env config

Blender MCP Tools
Get scene info & object data

Run scripts in Blender
Download/import assets
Apply materials & textures
Capture screenshots from viewport

🤝 Contributing
We welcome contributions! Please check out our CONTRIBUTING.md for:

-Code style guidelines

-Testing instructions

-Issue reporting

-Pull request process


🙏 Acknowledgments
   -🌀 Model Context Protocol for the MCP specification

   -🌄 PolyHaven for open 3D assets

   -🛒 Sketchfab for 3D model marketplace

   -🤖 Hyper3D Rodin for AI 3D model generation

   -🧱 Blender Foundation for the open-source 3D suite
