Deployment notes and fixes applied:
- Safe renderer attach/detach: src/utils/attachRendererToContainer.js and src/ar/components/ARViewer/WebXRManager.jsx
- GSAP parallax utility now returns cleanup function: src/animations/presets.js (gsapParallax3D)
- Shaders converted to JS string modules: src/shaders/*
- preserveDrawingBuffer disabled in renderers for better performance
- Basic Jest test to verify DOM attach/remove behavior included.

This package is a focused subset for running locally. For full production use, include the entire design-system, storybook, AR full stack and backend files.
