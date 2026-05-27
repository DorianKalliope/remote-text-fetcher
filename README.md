# Remote Text Fetcher

**Remote Text Fetcher** is a simple Visual Studio Code extension that fetches a text file from a configurable URL and displays its content in VS Code's output channel.

It runs automatically when VS Code starts, making it useful for checking status pages, reading remote notes, or monitoring simple text-based endpoints.

---

## 🚀 Features

- Fetches text content from any HTTP/HTTPS URL.
- Displays the fetched content in a dedicated output channel.
- Configurable URL – change it without modifying the extension.
- Runs silently in the background (no popups, no interruptions).

---

## 📦 Installation

### From the VS Code Marketplace

1. Open VS Code.
2. Go to the Extensions view (`Ctrl+Shift+X`).
3. Search for `Remote Text Fetcher`.
4. Click **Install**.

### Manual installation from VSIX

1. Download the `.vsix` file.
2. Run:  
   `code --install-extension remote-text-fetcher-0.0.1.vsix`

---

## ⚙️ Configuration

You can change the URL that the extension fetches:

1. Open VS Code Settings (`Ctrl + ,`).
2. Search for `remoteTextFetcher.url`.
3. Enter your desired URL (e.g., `https://example.com/status.txt`).

**Default value:** `http://localhost:3000/commands.txt`

---

## 📖 Usage

Once installed, the extension activates automatically when VS Code starts. It will:

- Fetch the content from the configured URL.
- Display the fetched text in the **"Remote Text Fetcher"** output channel (View → Output → select "Remote Text Fetcher").

The output channel shows the fetched content exactly as received from the server.

---

## 🛠️ Building from source

```bash
git clone <your-repo-url>
cd remote-text-fetcher
npm install
npm run compile
vsce package