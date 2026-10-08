# Base44 Setup Notes

## Project
Static single-page HTML site ("USWA FRIENDS — Batch 2024, Darul Huda Islamic University").
No build step, no dependencies, no backend.

## Running
Served via `nginx:alpine` in `docker-compose.base44.yml` on host port 3000.
The entry point is `sam.html` (configured as the nginx `index` in `nginx.base44.conf`).
A duplicate copy lives at `sam/sam.html` (identical to the root file).

## Verification
`curl http://localhost:3000/` should return the HTML page (title: "USWA FRIENDS - Batch 2024").
