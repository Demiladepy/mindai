MINDai 🧠

A collaborative multi-agent workspace assistant designed for remote teams.

Tech Stack

Meta LLaMA → Core language model for understanding, summarization, and Q&A.

Cerebras → Powers fast, efficient model inference.

Docker MCP Toolkit + Gateway → Runs and manages containerized agents smoothly.

ChromaDB → Handles long-term memory and semantic search.

Exa → Provides real-time external research capabilities.

LiveKit → Enables voice-based agent interaction.

Agents

Doc Parser Agent 📄 – Extracts and structures information from uploaded documents.

Summarizer Agent ✍️ – Condenses long texts into key takeaways.

Query Agent 🔍 – Handles user questions with context-aware responses.

Research Agent 🌐 – Enriches results using verified external data.

Voice Agent 🎤 – Engages in natural, voice-first conversations.

How It Works

Users upload documents → stored in S3 and indexed in ChromaDB.

Multiple agents process tasks in parallel for efficiency.

Cerebras and LLaMA collaborate to refine and optimize outputs.

The MCP Orchestrator intelligently routes tasks between agents.

The final, context-rich response is delivered via a chat interface or voice interaction.
