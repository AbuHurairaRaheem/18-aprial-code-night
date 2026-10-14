# HelpHub AI — Community Support Platform

HelpHub AI is a community-support prototype where members can create, discover, and respond to help requests. It pairs a Next.js/React frontend with a Node.js/Express API, MongoDB persistence, and rule-based request suggestions.

**Tech stack:** `Next.js` · `React` · `TypeScript` · `Tailwind CSS` · `Node.js` · `Express` · `MongoDB` · `Mongoose` · `JWT` · `REST API`

## Features in this snapshot

- Account registration and login with JWT-backed API authentication.
- Create, browse, filter, and manage community help requests.
- Request categories, urgency levels, and tags stored with the request.
- A frontend suggestion panel that proposes tags, categories, urgency, and sample rewrites based on simple keyword rules.

## AI implementation note

The “AI” suggestions in the current public source are mock/rule-based logic. The repository does **not** currently contain an external LLM API integration, retrieval-augmented generation, or lead-capture/lead-qualification workflow. Describe this project as a community-support prototype with rule-based suggestions, not as a deployed LLM or lead-qualification engine.

## Run locally

The application source is under `18-aprial-code-night/` in this repository.

1. Start the API:

   ```bash
   cd 18-aprial-code-night/backend
   npm install
   ```

   Create a `.env` file with `MONGODB_URL`, `JWT_SECRET`, `PORT=5000`, and `FRONTEND_URL=http://localhost:3000`, then run `npm run dev`.

2. Start the frontend in a second terminal:

   ```bash
   cd 18-aprial-code-night/frontend
   npm install
   ```

   Set `NEXT_PUBLIC_API_URL=http://127.0.0.1:5000/api` in the frontend environment, then run `npm run dev`.

The MongoDB URI and JWT secret must be supplied locally; never commit real secrets.

## Checks and deployment

The frontend production build and `npx tsc --noEmit` passed during review. No verified public Vercel deployment is currently linked to this repository; the project is source-only for now.
