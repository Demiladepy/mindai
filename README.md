# MINDai 🧠

MINDai is a collaborative multi-agent workspace assistant built to enhance how remote teams work, communicate, and access information. It operates as an intelligent system composed of multiple specialized AI agents—each designed to handle different aspects of teamwork such as document parsing, summarization, research, querying, and voice interaction.

By allowing these agents to collaborate in real time, MINDai helps distributed teams manage knowledge more effectively. Instead of manually searching through files, writing summaries, or switching tools, team members can simply interact with MINDai through chat or voice. The system coordinates multiple AI agents behind the scenes, processes data from documents and the web, and delivers accurate, context-aware insights.

In essence, MINDai acts as an AI-powered workspace companion—streamlining collaboration, reducing information overload, and ensuring remote teams stay aligned, informed, and productive.

# Tech Stack

Meta LLaMA → Core language model for understanding, summarization, and Q&A.

Cerebras → Powers fast, efficient model inference.

Docker MCP Toolkit + Gateway → Runs and manages containerized agents smoothly.

ChromaDB → Handles long-term memory and semantic search.

Exa → Provides real-time external research capabilities.

LiveKit → Enables voice-based agent interaction.

# Agents

Doc Parser Agent 📄 – Extracts and structures information from uploaded documents.

Summarizer Agent ✍️ – Condenses long texts into key takeaways.

Query Agent 🔍 – Handles user questions with context-aware responses.

Research Agent 🌐 – Enriches results using verified external data.

Voice Agent 🎤 – Engages in natural, voice-first conversations.

# How It Works

Users upload documents → stored in S3 and indexed in ChromaDB.

Multiple agents process tasks in parallel for efficiency.

Cerebras and LLaMA collaborate to refine and optimize outputs.

The MCP Orchestrator intelligently routes tasks between agents.

The final, context-rich response is delivered via a chat interface or voice interaction.
