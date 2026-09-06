# ShoeVista — CLAUDE.md

## Build / test / lint
- Client dev server: `npm run start` (in Testing/client) — runs `vite`
- Client build: `npm run build` (in Testing/client) — runs `vite build`
- Client preview: `npm run preview` (in Testing/client) — runs `vite preview`
- Client lint: `npm run lint` (in Testing/client) — runs `eslint . --ext js,jsx --report-unused-disable-directives --max-warnings 0`
- Server start: `npm run start` (in Testing/server) — runs `nodemon index.js`
- Server test: `npm run test` (in Testing/server) — currently a stub (`echo "Error: no test specified" && exit 1`)

## Rules observed
- Server uses ES modules (`"type": "module"` in Testing/server/package.json) — use `import`/`export`, not `require`
- The actual app code lives under `Testing/client` and `Testing/server`, not at the repo root — commands must be run from inside those subfolders

## Read first
- /Volumes/SIAM/Github Repos/ShoeVista/Testing/server/index.js
- /Volumes/SIAM/Github Repos/ShoeVista/Testing/client/src/main.jsx
- /Volumes/SIAM/Github Repos/ShoeVista/Testing/client/src/App.jsx

Architecture: see ARCHITECTURE.md — read before structural changes
