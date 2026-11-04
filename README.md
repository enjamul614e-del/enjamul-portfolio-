# Full-stack developer portfolio

## Project structure

```text
portfolio/
├── backend/
│   └── src/
│       ├── routes/
│       │   └── health.js
│       └── server.js
├── frontend/
│   ├── public/
│   │   └── images/
│   ├── src/
│   │   ├── index.css
│   │   └── index.js
│   └── index.html
├── package.json
└── README.md
```

## Run locally

1. Install the project dependencies from the portfolio root:

   ```sh
   npm install
   ```

2. Start the frontend in one terminal:

   ```sh
   npm run dev
   ```

   Vite prints the local URL, usually `http://localhost:5173`.

3. Start the backend in a second terminal:

   ```sh
   npm run dev:backend
   ```

   The Node.js API listens on `http://localhost:3001`. Check that it is running
   at `http://localhost:3001/api/health`.

The backend currently uses Node.js built-in modules, so it does not need a
separate dependency installation. Add API routes under `backend/src/routes/`.
Frontend source files belong in `frontend/src/`, and static assets belong in
`frontend/public/`.

## Build the frontend

```sh
npm run build
```

The production frontend is generated in `frontend/dist/`.
