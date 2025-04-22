# GPT-4.1 Web UI

A modern, private, and extensible web interface for OpenAI GPT-4.1 (including Vision), built with React and Vite.

## Features

- **Chat with GPT-4.1** using your own OpenAI API key
- **Persistent chat history** (text only, stored in your browser)
- **Upload images** (for GPT-4 Vision, if your API key supports it)
- **Upload files or folders** (text/code, with automatic chunking for large files)
- **Summarize codebases**: Summarize all uploaded files before sending to GPT-4.1
- **No backend required**: All data stays in your browser except API calls to OpenAI

---

## Getting Started

### 1. **Clone the repository**

```bash
git clone https://github.com/yourusername/gpt4-web-ui.git
cd gpt4-web-ui
```

---

### 2. Install dependencies

```bash
npm install
```

---

### 3. Start the development server

```bash
npm run dev
```

- The app will be available at [http://localhost:5173](http://localhost:5173) (or the port shown in your terminal).

---

## Usage

1. Enter your OpenAI API key (starts with ```sk-...```) in the field at the top.
   
2. Type your prompt in the text area.
   
3. Upload images (for GPT-4 Vision), files, or folders as needed.
   
4. (Optional) Summarize all files before sending to save tokens and improve results.
   
5. Click "Send" to chat with GPT-4.1.
    
6. Your chat history (text only) is saved in your browser for your next visit.

---

## Security & Privacy

- Your API key is only stored in your browser (localStorage) and is never sent anywhere except directly to OpenAI.
  
- Uploaded files and images are processed in your browser and are not persisted or uploaded anywhere except as part of your prompt to OpenAI.
  
- Chat history is stored as text only (no images or file contents) to avoid browser storage issues.

---

## Requirements

- [Node.js](https://nodejs.org/) v18 or newer recommended.

- An [OpenAI API key](https://platform.openai.com/account/api-keys) with GPT-4.1 access.

---

## Customization

You can edit ```src/App.jsx``` to change the UI, add features, or adjust chunking/summarization logic.
To deploy, build with ```npm run build``` and serve the ```dist``` folder with any static web server.

---

## License

[MIT](https://opensource.org/license/mit)

---

## Credits

- Built with [React](https://react.dev/) and [Vite](https://vitejs.dev/)
- Powered by [OpenAI GPT-4.1](https://platform.openai.com/docs/models/gpt-4.1)
