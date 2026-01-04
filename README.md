# Tech-Luxury 3D (packaged)

This archive contains a deployable subset of the TechnoLuxury 3D project:
- Frontend React app (Vite) with Three.js scene, UI components and styles.
- Design system core modules (tokens + a few 3D components).
- Critical bug fixes applied:
  - Safe append/cleanup of WebGL renderer canvas to avoid duplicate canvases and memory leaks.
  - GSAP parallax utility now returns a cleanup function to remove window event listener.
  - Shaders converted to JS modules exporting strings (no special bundler needed).
- Minimal Jest test for renderer attach behavior.

How to run (locally):
1. `npm install`
2. `npm run dev`
3. `npm run test` (to run the included test)

Files included are a focused subset for speed — expand as needed for full production.

Files added in this step:
- backend/ (Express API, Dockerfile, Prisma schema)
- docker-compose.yml and infra/nginx.conf
- design-system more components
- ARViewer index
- Storybook minimal config
- root Dockerfile to serve built frontend
