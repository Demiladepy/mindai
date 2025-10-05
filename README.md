# mindai 🧠

mindai is a collaborative multi-agent workspace assistant built to enhance how remote teams work, communicate, and access information. It operates as an intelligent system composed of multiple specialized AI agents—each designed to handle different aspects of teamwork such as document parsing, summarization, research, querying, and voice interaction.

By allowing these agents to collaborate in real time, mindai helps distributed teams manage knowledge more effectively. Instead of manually searching through files, writing summaries, or switching tools, team members can simply interact with mindai through chat or voice. The system coordinates multiple AI agents behind the scenes, processes data from documents and the web, and delivers accurate, context-aware insights.

In essence, mindai acts as an AI-powered workspace companion—streamlining collaboration, reducing information overload, and ensuring remote teams stay aligned, informed, and productive.

## Features

- **Multi-Agent Architecture**: Specialized AI agents working together seamlessly
- **Real-time Collaboration**: Team members can interact through chat or voice
- **Document Intelligence**: Upload and process documents with AI-powered insights
- **Voice Interaction**: Natural voice-based conversations with AI agents
- **Memory & Context**: Long-term memory storage with semantic search capabilities
- **External Research**: Real-time web research and data enrichment
- **Modern UI**: Beautiful, responsive interface built with Next.js and Tailwind CSS
- **Authentication**: Secure user management with Clerk integration

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

## Getting Started

### Prerequisites

- Node.js 18+ 
- npm or yarn
- Docker (for containerized agents)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/mindai.git
cd mindai
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
```bash
cp .env.example .env.local
# Edit .env.local with your configuration
```

4. Run the development server:
```bash
npm run dev
```

5. Open [http://localhost:3000](http://localhost:3000) in your browser.

## How It Works

1. **Document Upload**: Users upload documents → stored in S3 and indexed in ChromaDB
2. **Agent Coordination**: Multiple agents process tasks in parallel for efficiency
3. **AI Processing**: Cerebras and LLaMA collaborate to refine and optimize outputs
4. **Intelligent Routing**: The MCP Orchestrator intelligently routes tasks between agents
5. **Response Delivery**: The final, context-rich response is delivered via a chat interface or voice interaction

## Project Structure

```
src/
├── app/                    # Next.js app directory
│   ├── components/         # React components
│   ├── dashboard/          # Dashboard pages
│   ├── sign-in/           # Authentication pages
│   └── server/            # Server-side agents
├── components/            # Shared UI components
├── lib/                   # Utility libraries
│   └── orchestrator/      # MCP orchestrator
└── middleware.tsx         # Next.js middleware
```

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For support, email support@mindai.ai or join our community discussions.
