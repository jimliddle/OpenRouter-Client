# OpenRouter Modern Chat (Single-File PWA)

A fully-featured, beautifully designed modern chat client for the OpenRouter API, built entirely in a single, zero-dependency HTML file.

No build steps. No frameworks. No external CDNs. Just download, open in your browser, and start chatting with hundreds of LLMs.

## 🚀 Features

Zero Dependencies: Built with pure Vanilla HTML, CSS, and JavaScript. Everything, including SVG icons, is embedded.

True Single-File PWA: Dynamically generates its own manifest.json and Service Worker via Blob URLs, allowing you to install it as a native app on mobile or desktop directly from a single file.

100% Client-Side Privacy: Your API key, settings, and chat histories are stored securely and locally on your device using IndexedDB.

Multi-Threading: Organize your conversations with unlimited distinct chat threads.

Dynamic Model Switching: Fetches your available OpenRouter models on the fly. Switch models seamlessly mid-conversation—each AI response is individually tagged with the model that generated it.

Granular Message Control: Easily copy or delete individual prompts and responses.

Mobile-First Dark UI: A highly responsive, touch-friendly interface inspired by native dark mode applications.

"Danger Zone" Data Wipe: A one-click option to completely purge all local storage, threads, and API keys from your device.

## 🛠️ How to Use

Because this app requires zero build tools, getting started takes seconds:

- Clone or Download this repository.

- Open index.html in any modern web browser.

- Click on Settings & API in the sidebar.

- Enter your OpenRouter API Key and hit Save.

- Select a model and start chatting!

Installing as an App (PWA)

If your browser supports Progressive Web Apps (like Chrome, Edge, or Safari on iOS/Android):

- Open the file/URL in your browser.

- Look for the "Install App" button that dynamically appears in the sidebar (or use your browser's "Add to Home Screen" option).

- The app will be installed with a custom icon and will run in an immersive, standalone window.

## 🔒 Security & Privacy

This application is completely stateless on the server side (because there is no server!).

Storage: All data (including your API key) is stored using the browser's native IndexedDB API.

Network: The only network requests made are directly to https://openrouter.ai/api/v1/ to fetch models and send/receive chat completions. See OpenRouter for their privacy policy.

## 💻 Tech Stack

- HTML5 / CSS3: Custom, responsive layout using Flexbox and CSS variables.

- Vanilla JavaScript (ES6+): Modern JS utilizing async/await, fetch, and dynamic DOM manipulation.

- IndexedDB: Asynchronous local database wrapper for persistent state management.

- Blob URLs: Clever use of URL.createObjectURL to mount invisible Service Workers and Web Manifests without requiring actual separate files.

📄 License

This project is MIT licenses and free to use
