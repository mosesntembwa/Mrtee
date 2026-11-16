# Mr Tees (Moses Ntembwa) AI

## Setup
1. Install Node.js 18 or newer.
2. Moses's WhatsApp number (+260771043702) is already set in `public/config.js`. Change it there if it ever changes.
3. Copy `.env.example` to `.env` and add your Anthropic API key (console.anthropic.com).
4. Run: `node server.js` then open http://localhost:3000

## Files
- `public/index.html, style.css, app.js` - the chat screen (stars, greeting, 6 questions, chat history, new chat)
- `public/config.js` - WhatsApp number
- `knowledge.js` - everything the AI knows (services, fees, Moses, HELSB). Edit here to update prices or facts.
- `server.js` - keeps your API key secret and talks to Claude

## Hosting
Upload the whole folder to any Node host (Render, Railway, a VPS) and set the ANTHROPIC_API_KEY variable there. The key must never go inside the public folder.

## Notes
- WhatsApp number shows only when the AI talks about a service, a fee, or when someone asks for Moses.
- Chat history is saved on each customer's own phone/browser.
