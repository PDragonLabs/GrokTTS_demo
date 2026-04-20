# GrokTTS_demo
test for grok tts


How to Use It

Save as grok-tts-tuner.html.
Open via a local server (recommended): npx serve or python -m http.server 8000, then visit http://localhost:8000/grok-tts-tuner.html in Chrome/Edge.
Fill in your Ephemeral Client Secret (recommended for browser safety) or full Bearer token.
Choose voice, add expressive tags in the text box (e.g. [laugh], <whisper>, <slow>, etc.).
Click Speak with Grok TTS to hear high-quality results.
Use the browser section for instant free tuning when you don't want to call the API.

Important notes:

For real use, get an ephemeral token from your backend (calling POST https://api.x.ai/v1/realtime/client_secrets with your main API key). Direct main key use in browser is risky.
Grok TTS costs money based on characters — test with short text first.
The REST /v1/tts returns audio directly (MP3 by default).

If you want a full realtime voice chat version (mic input → Grok STT → LLM → Grok TTS) or a tiny Node.js backend to generate ephemeral tokens safely
