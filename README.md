# AI Chatbot Frontend

This is the frontend application for the AI Chatbot. It provides a sleek, modern chat interface built with React and Vite. The application communicates with the FastAPI backend to provide AI responses with real-time web search capabilities.

## Features

- **React 19 & Vite**: Fast development server and optimized build process.
- **Modern UI**: Clean and responsive chat interface with a premium design.
- **Markdown Support**: Renders AI responses using `react-markdown` for rich text formatting, including code blocks, lists, and links.
- **Loading States**: Visual indicators (loading dots) when waiting for the AI response.
- **Auto-scroll**: Automatically scrolls to the latest message as the conversation grows.

## Prerequisites

- Node.js (v18 or higher recommended)
- npm or yarn

## Installation

1. Navigate to the `frontend` directory:
   ```bash
   cd frontend
   ```
2. Install the dependencies:
   ```bash
   npm install
   ```

## Running the Application

Start the Vite development server:

```bash
npm run dev
```

The application will be available at `http://localhost:5173` (or the port specified by Vite).

## Configuration

The frontend is currently configured to communicate with the backend running on `http://localhost:8000`. If your backend is running on a different URL or port, update the `fetch` request URL in `src/App.jsx`:

```javascript
// In src/App.jsx
const response = await fetch('http://localhost:8000/api/chat', { ... });
```

## Building for Production

To create a production build, run:

```bash
npm run build
```

This will generate an optimized build in the `dist` folder, which can be served using any static file server.
