KALI AI v3 - SM

Features:
- Natural multi-turn AI chat
- Conversation history in the browser
- Hindi/Hinglish and English responses
- Voice input in supported browsers
- Read-aloud responses using browser speech synthesis
- SM context search from study-material, papers, courses and tests JSON
- Smart Library / Smart Timetable awareness
- Demo mode when no API key is configured

RUN:
1. Install Node.js 18+.
2. Open this backend folder in terminal.
3. Run: npm install
4. Set GEMINI_API_KEY as an environment variable.
5. Optional: set GEMINI_MODEL (default: gemini-2.5-flash)
6. Run: npm start
7. Open: http://localhost:3000/pages/kali.html

IMPORTANT:
Never put the API key inside frontend JavaScript. Keep it only as a server environment variable.
The browser voice features depend on browser/device support and permissions.
