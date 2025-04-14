# AI Agent with Gemini and MCP

A powerful AI agent implementation that combines Google's Gemini AI with Model Context Protocol (MCP) for enhanced context-aware interactions.

## 🚀 Tech Stack

- **AI Model**: Google Gemini 2.0 via `@google/genai` SDK
- **Context Protocol**: Model Context Protocol (MCP) via `@modelcontextprotocol/sdk`
- **Runtime**: Node.js (v18 or later)
- **Authentication**: Google Cloud Authentication

## ⚙️ Architecture

The project consists of two main components:

### Client
- Handles direct interactions with Gemini AI
- Manages chat history and conversation flow
- Implements MCP client for context management
- Uses SSE (Server-Sent Events) for real-time communication

### Server
- Implements MCP server functionality
- Provides context and tools to the AI model
- Handles resource management and tool execution

## 📋 Prerequisites

- Node.js v18 or later
- Google AI API key (from [Google AI Studio](https://aistudio.google.com/apikey))
- Environment variables configured

## 🛠️ Installation

1. Clone the repository
```bash
git clone <repository-url>
```

2. Install dependencies
```bash
# Install client dependencies
cd client
npm install

# Install server dependencies
cd ../server
npm install
```

3. Configure environment variables
```bash
# Create .env file in client directory
GEMINI_API_KEY=your_api_key_here
```

## 🚦 Usage

1. Start the MCP server:
```bash
cd server
npx nodemon index.js
```

2. Run the client:
```bash
cd client
npx nodemon index.js
```

## 🔑 Key Features

- Real-time AI interactions using Gemini 2.0
- Context-aware responses through MCP
- Streaming support for faster responses
- Tool integration capabilities
- Chat history management
- Secure API key handling

## 📚 Dependencies

### Client
- `@google/genai`: Google's Gemini AI SDK
- `@modelcontextprotocol/sdk`: MCP implementation
- `dotenv`: Environment variable management
- Various utility packages

### Server
- `@modelcontextprotocol/sdk`: MCP server implementation
- Standard Node.js modules

## ⚠️ Security Notes

- Never expose API keys in client-side code
- Use server-side implementations in production environments
- Follow Google Cloud security best practices

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

MIT License