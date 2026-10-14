# HelpHub AI — Frontend

A Next.js/React interface for a community-support platform where users can create and browse help requests. It connects to the repository’s Node.js/Express API and includes a prototype request-suggestion panel.

**Tech stack:** `Next.js` · `React` · `TypeScript` · `Tailwind CSS` · `Axios`

## Run locally

```bash
npm install
NEXT_PUBLIC_API_URL=http://127.0.0.1:5000/api npm run dev
```

Start the backend separately; setup instructions and API requirements are in the repository’s root README.

## Prototype note

The request-suggestion panel currently uses local keyword rules and mock copy. It does not call an external LLM API. No verified public Vercel deployment is linked yet.
