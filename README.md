# 🤖 Full-Stack AI Agent System using Model Context Protocol (MCP)

This project demonstrates a fully functional **AI Agent System** built from scratch using the **Model Context Protocol (MCP)** to enable **real-time DuckDuckGo web searches** via a Python CLI, orchestrated through the **Claude LLM**.

It showcases a modern approach to building **LLM-tool integrations** using a standardized communication protocol (MCP), dynamic tool calling, and local Flask server infrastructure.

---

## 🔍 Overview

The system allows a Claude-powered agent to perform real-time searches by interacting with external tools using the **MCP standard**. The agent can:
- Understand user queries
- Trigger structured tool calls
- Execute web searches using the DuckDuckGo API
- Return a summarized response back to the user

---

## 🧠 Core Features

- 🔄 **Real-time Tool Interaction** via Claude using MCP
- 🧩 **Model Context Protocol (MCP)** for standardized LLM-tool communication
- 🧠 **ClaudeClient + MCPClient** layers to manage structured requests
- 🌐 **DuckDuckGo API Integration** for live web search
- 🧪 **Natural Language → Structured Search Intent** conversion
- 🧰 **Flask-based MCP Server** for secure tool call handling

---

## 🏗️ Architecture

```bash
User Query
   ↓
Claude LLM ←→ ClaudeClient (CLI)
   ↓
MCPClient → Local Flask MCP Server
   ↓
Tool Execution Layer → DuckDuckGo API
   ↓
Results → MCPClient → Claude (Summarization) → User
