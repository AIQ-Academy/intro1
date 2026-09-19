# AIQ Academy Smart Chat v6 — DeepSeek

A multilingual AIQ Academy landing site with an in-page Academy assistant and a secure DeepSeek-powered assistant.

## Languages
- العربية
- English
- Français

## Start
```powershell
copy .env.example .env
# add DEEPSEEK_API_KEY to .env
node server.js
```
Open `http://localhost:5500`.

## DeepSeek
The server calls `https://api.deepseek.com/chat/completions`. Default model: `deepseek-v4-flash`.

Never expose your DeepSeek API key in frontend code.
