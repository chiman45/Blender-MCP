
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

