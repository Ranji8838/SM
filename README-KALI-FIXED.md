# SM – Students Material | Kali AI Fixed Edition

## Kali problem fixed

The earlier Kali page could show:

`Unexpected end of JSON input`

That happened when the browser tried to parse an empty or non-JSON server response with `response.json()`.

This edition fixes that in two places:

1. The frontend safely reads and validates the response before parsing JSON.
2. The backend always returns JSON for API errors.
3. If the backend is not running, Kali shows a demo response instead of silently failing.
4. When you use VS Code Live Server, Kali automatically tries the backend at `http://localhost:3000`.
5. When the Express server serves the page, Kali uses the normal `/api/kali` route.

## Fastest way to run

### Option A — Windows
Double-click:

`START-KALI.bat`

It installs the backend packages if necessary and starts the server.

Then open:

`http://localhost:3000/pages/kali.html`

### Option B — Terminal

Open a terminal inside:

`SM1/backend`

Run:

`npm install`

Then:

`npm start`

Open:

`http://localhost:3000/pages/kali.html`

## Full AI mode

The project is safe to use without an API key in demo mode.

For real AI replies, configure the key as an environment variable. Do NOT put the key inside `js/kali.js`.

Example environment values:

`GEMINI_API_KEY=YOUR_KEY`
`GEMINI_MODEL=gemini-2.5-flash`

The file `.env.example` is included as a template.

## Health check

After starting the backend, open:

`http://localhost:3000/api/health`

A working backend should return JSON containing:

`"ok": true`

## Important

This is a prototype. Before public deployment, use licensed/authorized educational content, authentication, privacy/security controls, rate limiting, logging/monitoring, backups and accessibility testing.
