# WebAI

WebAI is a lightweight AI chat workspace powered by the Groq API. It runs as a static website with no build step.

## Features
- Streaming AI responses
- Select from supported Groq models
- Multiple saved conversations with search and delete
- Custom system instructions and creativity control
- Stop generation and export conversations as text
- Responsive dark interface for desktop and mobile
- Browser-local storage for chats, preferences and API key

## Run locally
Open `index.html` in a modern browser.

## Connect Groq
1. Create an API key at https://console.groq.com/keys
2. Open **Settings & API key** in WebAI.
3. Paste your key and save.

**Security note:** the key is stored in this browser's localStorage and sent directly to Groq. Anyone with access to the browser profile can inspect it. Never commit or share your key. A public multi-user production service should use a backend proxy instead of exposing API keys in frontend code.

## Deploy to GitHub Pages
The repository includes a GitHub Actions workflow. In **Settings → Pages**, choose **GitHub Actions** as the deployment source. The workflow deploys the static site after pushes to `main`.
