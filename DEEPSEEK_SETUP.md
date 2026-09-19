# AIQ Academy + DeepSeek Smart Chat

## Two modes
1. **AIQ Academy Assistant** answers from the Academy page content in the browser and needs no API key.
2. **DeepSeek AI** calls `/api/chat` through the included Node server. The DeepSeek key stays on the server and is never placed in browser code.

## Security
Never put `DEEPSEEK_API_KEY` in `index.html`, browser JavaScript, or a public Git repository. Configure it only in the server `.env` file.

## Run on Windows PowerShell
```powershell
cd AIQ_Academy_Smart_Chat_v6
copy .env.example .env
# edit .env and add DEEPSEEK_API_KEY
node server.js
```
Then open `http://localhost:5500`.

## Model
The default model is `deepseek-v4-flash`. You can change it to `deepseek-v4-pro` in `.env`.

The website uses DeepSeek's OpenAI-compatible Chat Completions endpoint at `https://api.deepseek.com/chat/completions`.
