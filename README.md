# 🤖 AI Agent Project

## 📋 Overview

This project implements an intelligent AI Agent that connects to the Gemini 2.0 Flash model and provides tool functionality including Twitter posting capabilities. The project uses the Model Context Protocol (MCP) to facilitate communication between the client and server components.

## 🏗️ Project Structure

```
client/            # Frontend client implementation
  ├── index.js     # Client entry point with Gemini AI integration
  └── package.json # Client dependencies
server/            # Backend server implementation
  ├── index.js     # Server entry point with MCP and Express setup
  ├── mcp.tool.js  # Twitter integration tool
  └── package.json # Server dependencies
```

## ✨ Features

- 🧠 Integration with Google's Gemini AI model
- 🔄 Model Context Protocol for structured AI tool communication
- 🐦 Twitter posting capabilities
- 🧮 Simple calculation tools (addTwoNumbers)
- 💬 Interactive chat interface

## 🛠️ Prerequisites

- Node.js (v16 or higher)
- Twitter API credentials
- Google AI API key

## 📝 Environment Variables

Create a `.env` file in both the client and server directories:

**Client .env:**

```
GOOGLE_API_KEY=your_google_api_key_here
```

**Server .env:**

```
TWITTER_API_KEY=your_twitter_api_key
TWITTER_API_SECRET=your_twitter_api_secret
TWITTER_API_TOKEN=your_twitter_access_token
TWITTER_API_TOKEN_SECRET=your_twitter_access_token_secret
```

## 🚀 Installation

### Server Setup

1. Navigate to the server directory:

```bash
cd server
```

2. Install dependencies:

```bash
npm install
```

3. Create the `.env` file with your Twitter API credentials

### Client Setup

1. Navigate to the client directory:

```bash
cd client
```

2. Install dependencies:

```bash
npm install
```

3. Create the `.env` file with your Google API key

## 🏃‍♂️ Running the Application

### Start the Server

1. Open a terminal and navigate to the server directory:

```bash
cd server
```

2. Run the server:

```bash
node index.js
```

3. The server will start at http://localhost:3001

### Start the Client

1. Open another terminal and navigate to the client directory:

```bash
cd client
```

2. Run the client:

```bash
node index.js
```

3. The interactive chat interface will start in the terminal

## 💻 Usage

Once both the server and client are running:

1. The client will connect to the MCP server
2. You can interact with the AI through the terminal interface
3. The AI can use tools like posting to Twitter or performing calculations

## 🧩 How It Works

- The client connects to Google's Gemini AI and the MCP server
- The server provides tools to the client through the MCP protocol
- The client maintains a chat history and processes tool calls
- When a tool call is detected, it's forwarded to the server for execution

## 🔧 Available Tools

- **addTwoNumbers**: Performs addition of two numbers
- **createPost**: Posts a status update to Twitter

## 🤝 Contributing

Feel free to submit pull requests or create issues to improve this project.

## 📄 License

This project is licensed under the ISC License.
